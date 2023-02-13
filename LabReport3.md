# Lab Report 3
## Charisse Chua 

The command line I decided to research more about was `grep`. These are the 4 commands: 
1. `grep -i`
2. `grep -w`
3. `grep -o`
4. `grep -v`
***
**1.** `grep -i`


`grep -i "PuertoRico" demoResults.txt` output:
<a href='https://www.linkpicture.com/view.php?img=LPic63ea6c1c8e7751955032355'><img src='https://www.linkpicture.com/q/Screenshot_20230213_085546.png' type='image'></a>

`grep -i "puertorico" demoResults.txt` output:
<a href='https://www.linkpicture.com/view.php?img=LPic63ea6cf5d81e595053389'><img src='https://www.linkpicture.com/q/Screenshot_20230213_090058.png' type='image'></a>

`grep -i` ignores the case when searching for matching characters. This can be helpful because when you're searching for terms, you don't always know what the case is/don't need the case to match. In the second example, when I used just regular grep to search, it showed there were no files that matched that which can be misleading. 

**2.** `grep -w` 

`grep -r -w "some" written_2` vs `grep -r "some" written_2` output:

`grep -r -w "some" written_2`
<a href='https://www.linkpicture.com/view.php?img=LPic63ea6e926f1d01905104765'><img src='https://www.linkpicture.com/q/Screenshot_20230213_090649.png' type='image'></a>

`grep -r "some" written_2`
<a href='https://www.linkpicture.com/view.php?img=LPic63ea6e926f1d01905104765'><img src='https://www.linkpicture.com/q/Screenshot_20230213_090554.png' type='image'></a>

`grep -r -w "something" written_2` output:
<a href='https://www.linkpicture.com/view.php?img=LPic63ea6e926f1d01905104765'><img src='https://www.linkpicture.com/q/Screenshot_20230213_090554.png' type='image'></a>

When just using the regular `grep -r "some"` to recursively search for the word through all the files in written_2, it displays all of the words that have "some" in it, even if it's a substring. The output was difficult to document, but from the screenshot you can see that both "sometimes" and "something" were included. If I wanted to just search for the word "some" and no other words where "some" is a substring, then it is helpful to use `grep -w`. It will search for only when that word stands alone, not when it's part of another word.


**3.** `grep -o` 


`grep -r -o "nowhere" written_2` output:
<a href='https://www.linkpicture.com/view.php?img=LPic63ea7075f179b922907660'><img src='https://www.linkpicture.com/q/Screenshot_20230213_091534.png' type='image'></a>

`grep -r "nowhere" written_2` output:
<a href='https://www.linkpicture.com/view.php?img=LPic63ea7075f179b922907660'><img src='https://www.linkpicture.com/q/Screenshot_20230213_091534.png' type='image'></a>
In the first example, when I use `grep -o` it shows just the file names and the matching word. It doesn't display all the lines before/after it. This can be helpful when you just want to see the matching word directly next to the file name. It makes it much cleaner and less data to sort through. If you look at the second example where there is no `grep -o`, it displays all the surrounding lines around the word you're searching for, which is difficult to analyze and not always necessary. 

**4.** `grep -v`

`grep -v "txt" demoResults.txt` output: 
<a href='https://www.linkpicture.com/view.php?img=LPic63ea73092df7f2098461673'><img src='https://www.linkpicture.com/q/Screenshot_20230213_092529.png' type='image'></a>


`grep -v "travel-guides" demoResults.txt` output: 
<a href='https://www.linkpicture.com/view.php?img=LPic63ea73092df7f2098461673'><img src='https://www.linkpicture.com/q/Screenshot_20230213_092529.png' type='image'></a>

`grep -v` searches for lines that don't match the given pattern/string. In the first example, it prints only the file names that don't have "txt". This can be helpful if you are searching through files and don't want a certain type of file to be returned, such as ".txt" or ".java". The second example returns only the file names that aren't in "travel-guides." This can also be helpful if you want to sort through different directories so that you can sort out what you don't want to have.

Source: https://www.geeksforgeeks.org/grep-command-in-unixlinux/
