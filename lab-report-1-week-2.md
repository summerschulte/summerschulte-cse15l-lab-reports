# How to Log Into Course-Specific ieng6 Account
## Step 1: Download **Visual Studio Code**
[This](https://code.visualstudio.com/) website will give directions on how to install VSC onto your computer. There are directions for all kinds of platforms (windows/mac) etc. 
https://summerschulte.github.io/summerschulte-cse15l-lab-reports/lab-report-1-week-2.md

![Image](VSdownload.png)

## Step 2: Remotely Connecting
Connecting your machine to connect to a remote computer. This is important so that you can do work on multiple computers.
### Install **SSH**
[This](https://docs.microsoft.com/en-us/windows-server/administration/openssh/openssh_install_firstuse) website will give directions for installing SSH.

### Look up your account

[This](https://sdacs.ucsd.edu/~icc/index.php) website will have you login to your UCSD account and get your username.

### Open Visual Studio Code
- Open a terminal (Terminal -> New Terminal)
- Type "$ ssh cs15lsp22zz@ieng6.ucsd.edu" into the command line. *Replace* "zz" with your account letters.
- It will ask you a yes/no question about continuing since it is your first time connecting. Type *yes*.
- Enter your password.

It should look something like this:
![Image](SS.png)

We will call your computer the *client* and the computer in the lab the *server*.

## Step 3: Run Some Commands
We will now try running some basic commands and observe their output! It's okay if some cause errors, try to figure out why these instances occur.

Try these on your computer and the remote computer after ssh-ing:

- cd
- ls
- pwd
- mkdir
- cp

Observe the results.

Now try these!

- cd  ~
- cd
- ls -a
- ls </home/linux/ieng6/cs15lsp22/cs15lsp22abc>     Replace 'abc' with someone in your group's username.
- cp /home/linux/ieng6/cs15lsp22/public/hello.txt ~/
- cat /home/linux/ieng6/cs15lsp22/public/hello.txt

**Here is an example output**
![Image](commands.png)

---
### *To log out:* Ctrl-D

## Step 4: Moving Files over SSH with scp

This is an important step as you will learn how to *work remotely* and copy files between computers. This is useful because you may want to work both locally and remotely!

The command to do this is called **scp**. 