# Lab 1 Report!
This report will go over the steps on how to install the Visual Studio Code (**VS Code**) text editor, remotely connect to the course-specific ieng6 account (student specific account in a remote computer), and cover some basic git commands through the git bash terminal on VS Code.

## Installing VScode
1. Go to the Visual Studio Code website https://code.visualstudio.com/
2. Click on the Blue Download Button on the top right of the web page. 
3. Download the appropriate Visual Studio Code file based on the operating system of your device (i.e. Windows (PC) or OSX (Mac)).
<img width="889" alt="image" src="https://user-images.githubusercontent.com/85651103/212216789-8cd5a546-41b5-4fec-9543-2d86b920e28c.png">
4. After downloading, just install using the basic settings onto your device. The display can be different depending on your operating system. This is an example of what your home page may look like (for Windows).

<img width="665" alt="image" src="https://user-images.githubusercontent.com/85651103/212217455-4ab1f25c-f29a-4215-ace4-5a70b6645731.png">

## Remotely Connecting
There is a course-specific remote server account for each student in CSE 15L. The following steps are to access and connect to your student remote-server account by connecting VScode to a terminal.

1. If your device is using a Windows operating system, you need to download a terminal Git Bash.
a) Install Git here: https://gitforwindows.org/
b) Follow these instructions in order to open and set the installed **git bash** as the VScode terminal: https://stackoverflow.com/questions/42606837/how-do-i-use-bash-on-windows-from-the-visual-studio-code-integrated-terminal/50527994#50527994

Your terminal on VScode should looking like this: on the top-right there is a tab that will say bash on it if the git bash terminal is open.
<img width="918" alt="image" src="https://user-images.githubusercontent.com/85651103/212225745-bf61ae91-b394-454d-9c3a-4ab787a2de10.png">

2. Log into to this website in order to access the student remote server account: https://sdacs.ucsd.edu/~icc/index.php

Once logged in, you should reach a page like this: Your course-specific account name resides in the bolded box ('cs15lwi23zz' with 'zz' being the letters in your course-specific account.)
<img width="416" alt="image" src="https://user-images.githubusercontent.com/85651103/212226340-f9afe89e-3bf4-49d4-9715-c8be4c2d8115.png">

3. In the opened terminal on VScode, use the ssh command to connect to remote server.
**$ ssh cs15lwi23zz@ieng6.ucsd.edu**

If it's the first time connecting to the server, there may come a message as so:
**⤇ ssh cs15lwi23zz@ieng6.ucsd.edu
The authenticity of host 'ieng6.ucsd.edu (128.54.70.227)' can't be established.
RSA key fingerprint is SHA256:ksruYwhnYH+sySHnHAtLUHngrPEyZTDl/1x99wUQcec.
Are you sure you want to continue connecting (yes/no/[fingerprint])?**

Type yes and press enter

4. Type in your password (You will not see the characters when they are being typed, but they are being entered)

If you password doesn't work, you likely need to reset your password using the following instructions
- log in here: https://sdacs.ucsd.edu/~icc/index.php
- click on your course-specific account name (the block starting with 'cs15lwi23')
- click on 'change your password' and then change your password (one that is more complicated than your last one would work better)
- wait ~15-20 minutes and then repeat step 3

You should see something like this if successfully logged into the remote server!
<img width="400" alt="image" src="https://user-images.githubusercontent.com/85651103/212228134-3950d75a-3b0f-44cd-8cf8-a169bb314b31.png">

## Trying Some Commands
Here are some commands to test out and experiment with after you have connected your terminal to your remote server.
Some basic/common commands to try:
- cd OR cd ~ - changes the directory you are in
- ls - will list all files that are in your directory
- cp /home/linux/ieng6/cs15lwi23/public/hello.txt ~/ - will copy the file from the directory or file path that is indicated into my home directory
- cat /home/linux/ieng6/cs15lwi23/public/hello.txt - read out or print to the screen the text that is located within a particular text file
- **mkdir <dir name>** - will create a directory within your current directory

For example, after running some of the above commands, you may get an output like this:
  <img width="445" alt="image" src="https://user-images.githubusercontent.com/85651103/212229842-716ec266-e455-448a-b8c0-93fd0c104a5d.png">

In order to log out of the remote server you can
1. Run Ctrl-D command
2. Run **exit** on terminal
  
  
This is the end of this tutorial! I hope that it helped you to log into your course-specific account and test out some commands on your terminal!
