# **Week 1 Lab Report**
**Charisse Chua**

## Installing VS Code
1. Go online to the [VS code website](https://code.visualstudio.com/) and follow the instructions to download it from there.
2. After downloading it you should be able to open up a blank file like this: 
  ![Image](https://www.linkpicture.com/q/Screenshot-125_1.png)
  This can be done by clicking *file* in the top left corner, and *New file*
(I had already installed VS code on my laptop before, so that is why there are other files open in the picture)

## Remotely Connecting 
1. Install [git for windows](https://gitforwindows.org/)
2. Open the terminal by clicking *terminal* -> *new terminal* or using keyboard shortcut Ctrl or Command + `
3. Type ```ssh cse15lwi22fff@ieng6.ucsd.edu``` (replace fff with the 3 unique letters of your ID. If you don't know your ID it can be found [here](https://sdacs.ucsd.edu/~icc/index.php))
4. There is a high chance that you will get a message that says 
```⤇ ssh cs15lwi23zz@ieng6.ucsd.edu
The authenticity of host 'ieng6.ucsd.edu (128.54.70.227)' can't be established.
RSA key fingerprint is SHA256:ksruYwhnYH+sySHnHAtLUHngrPEyZTDl/1x99wUQcec.
Are you sure you want to continue connecting (yes/no/[fingerprint])?
```
5. After typing ```yes``` it should prompt you to enter your password, and then this screen should appear: 
![Image](https://www.linkpicture.com/q/Screenshot-126_1.png)
6. By logging in this means that you now have remote access!

## Trying Some Commands
1. There are several commands that you can type into the terminal 
* ```mkdir``` - creates a new folder in the directory. If a folder with the name already exists it won't let you create one.  
* ```ls``` - displays all the folders in the directory
* ```pwd``` - prints the current working directory 
* ```cd``` - changes the directory to whatever comes after ```cd```. For example ```cd ..``` takes out the directory back another layer. 
Here are some examples of the commands being used in a terminal: 
![Image](https://www.linkpicture.com/q/Screenshot-127.png)

2. To log out of the server you can use Ctrl-D and then run ```exit```
