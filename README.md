# Linux-fundamentals
This repo is for anyone with an interest in picking up Linux. 

Over the Wire Bandit game
In Level 0 you need to connect to the SSH host  bandit.labs.overthewire.org. 
ssh username@ bandit.labs.overthewire.org -p 2220
the password is located in a file in home directrory , the password is ZjLjTmM6FvvyRnrb2rfNWOZOTa6ip5If
You need to Exit the SSH and log on using bandit1 username and the above password

In level 1 there is a dashed file , you need to use the command cat ./- to view the contents of the file
the file contains the password 263JGJPfgU6LtdEvgfWU1XP5yac29mFx

In level 2 the password is in a file with spaces in this filename, called spaces in this filename
Wrap the filename around "" to refer to this file
Password MNk8KNH3Usiio41PRUEoDFPqfxLPlSmx

Level 3 contains a hidden directory, you need to use ls -a to show
cd to that directory and you will see it is empty. Again use ls -a to show a hidden file.
The password is 2WmrDFRmJIq3IPxneAaMGhap0pFhF3NJ

In Level 4 there are 9 files. Only 1 is "human-readable". Find this file using find -type f | xargs file | grep text
outputs file07 and use cat ./ to rread it. the password is 4oQYVPkxZOOEOO5pTW81FB8j8lxXGUQw


