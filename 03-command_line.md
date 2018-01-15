# Learn command line

Please follow and complete the free online [Bash Scripting Tutorial](https://ryanstutorials.net/bash-scripting-tutorial/) or [Codecademy's Learn the Command Line](https://www.codecademy.com/learn/learn-the-command-line). These are helpful tutorials. You should be able to go through these in a couple of hours.

**Note:** Bash is not installed on a PC. Rather, PC users must install Cygwin. Once Cygwin has been installed, the command line interface witll _emulate_ bash. You can find all information regarding Cygwin [here](https://www.cygwin.com/).

---

### Q1.  Cheat Sheet of Commands  

Here's a list of items with which you should be familiar:  
* show current working directory path
* creating a directory
* deleting a directory
* creating a file using `touch` command
* deleting a file
* renaming a file
* listing hidden files
* copying a file from one directory to another

Make a cheat sheet for yourself: a list of at least **ten** commands and what they do.  (Use the 8 items above and add a couple of your own.)  

Command | Description
------------ | -------------
ls | how files
mv | move a file
man | help doc for a command
locate | find a file
clear | clear terminal screen
tar | create archive
grep | regex file contents
ssh | login to remote
awk | parse text files
diff | compare difference between two text files
sort | sort file contents
chmod | change permissions

---

### Q2.  List Files in Unix   

What do the following commands do:  
`ls`  
`ls -a`  
`ls -l`  
`ls -lh`  
`ls -lah`  
`ls -t`  
`ls -Glp`  

Command | Description
------------ | -------------
`ls` | list files in directory
`ls -a` | + hidden files too
`ls -l` | + shows file detail info
`ls -lh` | + same as above but the size column is more readable with appropriate units
`ls -lah` | + same as above but also includes hidden files
`ls -t` | + sort files by mod date in asc order
`ls -Glp` | + file details and add a slash at the end of directory names

---

### Q3.  More List Files in Unix  

Explore these other [ls options](http://www.techonthenet.com/unix/basic/ls.php) and pick 5 of your favorites:

> r, R, u, m, t

---

### Q4.  Xargs   

What does `xargs` do? Give an example of how to use it.

> Helps execute commands by passing in an argument list
> find ./Desktop -print | xargs grep "ls"


 

