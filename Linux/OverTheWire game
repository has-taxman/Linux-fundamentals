# Linux-fundamentals
This repo is for anyone with an interest in picking up Linux. 

**Over the Wire Bandit game**
In Level 0 you need to connect to the SSH host  bandit.labs.overthewire.org. 
ssh username@ bandit.labs.overthewire.org -p 2220
the password is located in a file in home directrory , the password is ZjLjTmM6FvvyRnrb2rfNWOZOTa6ip5If
You need to Exit the SSH and log on using bandit1 username and the above password

In level 1 there is a dashed file , you need to use the command cat ./- to view the contents of the dashed file
the file contains the password 263JGJPfgU6LtdEvgfWU1XP5yac29mFx

In level 2 the password is in a file with spaces in this filename, called spaces in this filename
Wrap the filename around "" to refer to this file
Password MNk8KNH3Usiio41PRUEoDFPqfxLPlSmx

Level 3 contains a hidden directory, you need to use ls -a to show
cd to that directory and you will see it is empty. Again use ls -a to show a hidden file.
The password is 2WmrDFRmJIq3IPxneAaMGhap0pFhF3NJ

In Level 4 there are 9 files. Only 1 is "human-readable". Find this file using find -type f | xargs file | grep text
outputs file07 and use cat ./ to read it. the password is 4oQYVPkxZOOEOO5pTW81FB8j8lxXGUQw
Another easier method of finding this file is $ find ./*
This list the file types of all the files in the current directory.

In level 5 you need to use the find again, this time search for  a file exactly 1033bytes
use find . -type f -size 1033c
Password HWasnPhtq9AVKe0dmk45nxy20cvUa6EG

In level 6 more on the find command. This time we learn how to search by -user and -group and -size
$ find / -type f -user bandit7 -group bandit6 -size 33c 2>/dev/null
morbNTDkSW6jIlUc0ymOdMaLnOlFVAaj

In level 7 we use the comman grep to search for the word (pattern) "millionth". the word needs to be quoted
dfwvzFQi4mU0wfNbFOe9RoWskMLg7eEc

In level 8 you need to find a pattern of characters that only occurs once.
grep "pattern" filename: Searches for the pattern in the file.
sort: Sorts the output so identical lines are grouped together.
uniq -c: Counts the occurrences of each unique line and prefixes the count to each line.
grep "^ *1 ": Filters lines where the count is exactly 1.
The -o option in grep ensures that only the matched pattern (word) is printed, not the entire line.
Adjust the pattern (\w\+ in this case) to match your specific needs.
Use the command $ grep -o "\w\+" data.txt | sort | uniq -c | grep "^ *1 " 
Password 4CKMh1JI91bUIZZPXDqGanal4xvAg0JM


In level 9 you need to search for heman-readble string , preceeded by = signs.
use $ strings filename | grep "[A-Za-z0-9]"
FGUW5ilLVJrxX9kMYMmlN4MgbpfMiqey

In level 10 you need to decode the base64 text
$ base64 -d data.txt
The password is dtR173fZKb0RRsDFSGsg2RWnpNVj3qRr

In level 11 the dext has been rotated by 13 positions, meaning each character has been swapped for a character 13 positions ahead in the alphabet
$ cat data.txt | tr 'A-Za-z' 'N-ZA-Mn-za-m'
The password is 7x16WNeHIi5YkIhWsfFIqoognUTyj9Q4

In level 12 you have a hexdump of a file that has been repeatedly compressed. use the $ file data.txt command to find out how this file has been compressed e.g gzip
use $ gunzip -c data.txt > unzipped_data.txt
and repeat this process until you find the file which has ASCII text
FO5dwFsc0cbaIiH0h8J2eUks2vdTDwAn

In level 13 you are given an ssh private key. You need to use this to access the bandit14 user via ssh. Only bandit14 can access the file which contains the key due to file permissions. You do not have sudo permissions. use command $ ssh -i sshkey.private bandit14@localhost -p 2220
Password is MU4VWeTyJk8ROof1qqmcBPaLh7lDCPvS

In level 14 you need to submit the password for level 14 when you join the localhost on port 30000
use the nc command $ nc localhost 30000
Password for level 15 is 8xCjnmgoKbGLhHFAZlGE5Tmu4M2tKJQo

In level 15 you need to connect to port 30001 on localhost which is using SSL/TLS encryption and submit the previous password
Use command $  openssl s_client -connect localhost:30001
kSkvUpMQ7lBYyCM4GBPvCvT1BfWRy0Dx

In level 16 submit the current password to a port on localhost in the range 31000 to 32000. First find out which of these ports have a server listening on them. Then find out which of those speak SSL/TLS and which don’t.
User $ nmap localhost -p 31000-32000   to list which servers listening
Then check which of them have speak SSL/TTLS using $ ncat --ssl localhost portnumber and past the current password
The output is a private key. Copy the private key. Exit SSH server
Create a file and call it key $ vim key
Paste in the key
Now log in to the ssh using the key (same as level 13)
$ ssh -i key bandit17@bandit.labs.overthewire.org -p 2220

In level 17 you need to compare files using the diff command. Result shows where the files have changed, password is x2gLTTjFwMOhQ8oWNbMN362QKxfRqGlO

In level 18 you get a message "BYEBYE! Connection to bandit.labs.overthewire.org closed." on the end of the welcom message to the ssh.
The .bashrc (shell) has been modified to log you out when you log in with SSH
use the command $ ssh -t bandit18@bandit.labs.overthewire.org -p 2220 /bin/sh
The password is in the readme file cGWpMaKXVwDUNgPAVJbWYuGHVn9zl3j8

In level 19 you are given the setuid binary. Execute this using $ ./ 
Find the password in $./bandit20-do cat /etc/bandit_pass/bandit20
0qXahG8ZjOVMN9Ghs7iOWsCfZyXOUbYO
