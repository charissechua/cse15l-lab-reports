# Lab Report 5
Charisse Chua


I decided to do what we did in lab report 3, except I am now exploring the `find` command instead of the `grep` command. 
***

These are the four commands I am testing:
1. `find ./GFG -name sample.txt`
2. `find ./GFG -empty`
3. `find . -type f -name "*.txt"`
4. `find /tmp -type f -name ".*"`


## 1. `find ./directory -name sample.txt`
Finds the file with that specific name within that specified directory. In my case, I went into the skill-demo1-data directory and searched for that specific text file and received the following output.

`find ./GFG -name something.txt` output: 

`./skill-demo1-data/something.txt`

## 2. `find ./directory -empty`
Finds the files/folders in the given directory that are empty. In my case, I searched through the skill-demo1-data library to find the empty files.

`find ./skill-demo1-data -empty` output:
```./skill-demo1-data/.git/branches
./skill-demo1-data/.git/refs/tags
./skill-demo1-data/.git/objects/info
./skill-demo1-data/written_2/demoResults.txt
```

## 3. `find . -type f -name "*.txt"`

Finds all the files that ends in the given extension. In this case, I searched through the skill-demo1-data library to find all the files that ended in `.txt` and received the following output: 

`find . -type f -name "*.txt"` output (shortened):
```./written_2/non-fiction/OUP/Abernathy/ch1.txt
./written_2/non-fiction/OUP/Abernathy/ch14.txt
./written_2/non-fiction/OUP/Abernathy/ch15.txt
./written_2/non-fiction/OUP/Abernathy/ch2.txt
./written_2/non-fiction/OUP/Abernathy/ch3.txt
./written_2/non-fiction/OUP/Abernathy/ch6.txt
./written_2/non-fiction/OUP/Abernathy/ch7.txt
./written_2/non-fiction/OUP/Abernathy/ch8.txt
./written_2/non-fiction/OUP/Abernathy/ch9.txt
./written_2/non-fiction/OUP/Berk/CH4.txt
./written_2/non-fiction/OUP/Berk/ch1.txt
./written_2/non-fiction/OUP/Berk/ch2.txt
./written_2/non-fiction/OUP/Berk/ch7.txt
./written_2/non-fiction/OUP/Castro/chA.txt
./written_2/non-fiction/OUP/Castro/chB.txt
./written_2/non-fiction/OUP/Castro/chC.txt
./written_2/non-fiction/OUP/Castro/chL.txt
./written_2/non-fiction/OUP/Castro/chM.txt
./something.txt
```
## 4. `find /tmp -type f -name ".*"`

Finds all hidden files. I did this on the skill-demo1-data directory and got the following output: 

`find /tmp -type f -name ".*"` output (shortened):
```find: '/tmp/cs120wi23mm-pulse': Permission denied
find: '/tmp/cs120wi23al-pulse': Permission denied
find: '/tmp/yuw571-pulse': Permission denied
find: '/tmp/srustagi-pulse': Permission denied
find: '/tmp/cs15lwi23awd-pulse': Permission denied
find: '/tmp/cs120wi23ii-pulse': Permission denied
find: '/tmp/h7shi-pulse': Permission denied
find: '/tmp/cs120wi23ni-pulse': Permission denied
find: '/tmp/ee15wi23an-pulse': Permission denied
find: '/tmp/ee15wi23gf-pulse': Permission denied
find: '/tmp/cs15lwi23aik-pulse': Permission denied
find: '/tmp/cs120wi23aj-pulse': Permission denied
find: '/tmp/cs120wi23ej-pulse': Permission denied
find: '/tmp/cs15lwi23aqw-pulse': Permission denied
``` 
Clearly, there were many hidden files that I was not able to access, but at least with this command now I know it exists.

Sources: https://www.geeksforgeeks.org/find-command-in-linux-with-examples/
https://www.tecmint.com/35-practical-examples-of-linux-find-command/
