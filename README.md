# Necessary Linux Commands


## Basic Commands
1. `ls`: List all the files
   1. `ls -l`
   2. `ls -ltr`
2. `mkdir` : Create a directory
3. `touch` : Create a file
4. `free -h` : Show memory usage in Gi
5. `df -h` : Show info of disks
6. `date` : Show the current date
7. `pwd`
8. `clear`
9.  `cd`
10. `rm`
11. `rm -r`
12. `rmdir`
13. `cat demo.txt`
14. `echo "hello"`
15. `echo "hello" > demo.txt`
16. `zcat`
17.  `head` : prints first 5 lines
     1. `head -f demo.txt` : monitors and prints
     2. `head -n 7 demo.txt` : prints top 7 lines from demo.txt
18.  `tail` : prints last 5 lines
     1. `tail -f demo.txt` :
19. `less`: prints long file by pages
20. `more`:
21. `cp file_name destination/`:
    1.  `cp -r `
22. `mv`
23. `wc demo.txt` : word count , outputs as `lines words bytes` eg: `1 45 200`
24. `ln /path_of_the_file shortcut_name` : hard link
    1. `ln -s /path_of_the_file shortcut_name` : soft link 
    2. **use `ls -ltr` to list files with soft links**
25. `cut demo.txt` : cut content from the file `demo.txt`
    1.  `cut -b 1 demo.txt` : cut 1 byte from `demo.txt`
    2.  `cut -b 1-1 demo.txt` : cut 1st 4 bytes from `demo.txt`
26. `echo "hello" | tee hello.txt` : prints "hello" and insert the printed content into "hello.txt"
27. `sort demo.txt` : sorts the content of `demo.txt` alphabetically
28. `diff hello.txt demo.txt` : difference between hello.txt and demo.txt (maximum 2 params)

## SSH Commands
29. `chmod 400 private-key.pem` : to use without `sudo`
30. `ssh -i private-key.pem username@hostname` then enter `yes` : connect to remote machine. here `hostname` is the ***Public DNS*** of the remote machine.

## Advance Commands
31. `du` : disk utility
32. `top` : show all running processes
33. `ps` : show process info with id
34. `fuser` : 
35. `kill` : kill a processs
    1. example:  `kill -9 process_id`
36. `nohup` : inserts the printed content of a command to a file
    1.  example: `nohup ls` prints the output of `ls` to a file named `nohup.out`
    2.  **useful for logging**
