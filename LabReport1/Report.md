# Lab Report 1: Remote Access and File System
---
## Step 1: Installing VScode
1. Go to this link: [the Visual Studio Code website](https://code.visualstudio.com/) and click download to install Visual Studio Code on your computer
![VSCode Download Screen](VSCodeDownloadSS.png)
2. Follow the instructions to complete the installation process and open VScode, the window should look similar to the image below
![VSCode Welcome Screen](VSCodeSS.png)
*Note: As I already had Visual Studio Code installed on my computer, I did not need to follow these setup instructions and just opened the application directly*
## Step 2: Remotely Connecting
1. If you're using a Windows computer, ensure that you have [Git for Windows](https://gitforwindows.org/) installed
![Git for Windows Website](Git4WindowsSS.png)
2. Once Git is installed, follow [these instructions from this post on Stackoverflow](https://stackoverflow.com/questions/42606837/how-do-i-use-bash-on-windows-from-the-visual-studio-code-integrated-terminal/50527994#50527994) to begin using Bash in the VSCode terminal
3. Open the VSCode Terminal (by typing Ctrl or Command + \`) 
4. Now you can write your commands into the terminal, when you see the `$` that is the convention for where you will be writing your commands
5. To connect remotely to one of the computers in the CSE Basement (your sesrver), you first type this command into the terminal: `$ ssh cs15lsp23xx@ieng6.ucsd.edu` where `xx`is replaced by the last 2 letters in your own course-specific account
6. If you're logging into your account for the first time, you will be prompted `Are you sure you want to continue connecting (yes/no/[fingerprint])?`, type `yes` and then enter
7. Type in your password when prompted
8. Upon logging in and successfully remotely connecting, you will receive output similar to this:
 ```
 Hello cs15lsp23if, you are currently logged into ieng6-202.ucsd.edu

 You are using 0% CPU on this system

 Cluster Status 
 Hostname     Time    #Users  Load  Averages  
 ieng6-201   12:30:01   9   0.04,  0.28,  0.25
 ieng6-202   12:30:01   14  1.58,  0.69,  0.38
 ieng6-203   12:30:01   7   0.26,  0.37,  0.27


 Thu Apr 06, 2023 12:33pm - Prepping cs15lsp23
 ```
*Note: Since I had difficulties trying to remotely connect to the server when writing this report (terminal saying that the connection was closed), I was only able to use copied and pasted output that I produced during the lab instead of using a new screenshot*
## Step 3: Trying Some Commands
1. Test out some commands on your computer and on the remote computer
2. Here are some commands you can try:
* `cd`
* `cd ~`
* `ls`
* `ls -lat`
* `ls -a`
* `ls /home/linux/ieng6/cs15lsp23/cs15lsp23xx` (`xx` is the last 2 letters of someone else's account)
* `pwd`
* `mkdir`
* `cp`
* `cp /home/linux/ieng6/cs15lsp23/public/hello.txt ~/`
* `cat /home/linux/ieng6/cs15lsp23/public/hello.txt`
![Testing Commands](TestingCommandsSS.png)
*An example of testing out some commands*
3. When you are done testing commands, logout by typing Ctrl-D or `exit` in the terminal



