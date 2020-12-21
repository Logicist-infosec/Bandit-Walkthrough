# Level 6 --> Level 7

> ## Level Goal
> The password for the next level is stored somewhere on the server and has all of the following properties:
> * owned by user bandit7
> * owned by group bandit6
> * 33 bytes in size
> ## Commands you may need to solve this level
> ls, cd, cat, file, du, find, grep

## Answer
1. Execute `find / -group bandit6 -user bandit7 -size 33c 2>&1 | grep -vi "permission denied" | grep -vi "no such file or directory"` to find the password file.
2. Run `cat <password file>` to get password 
"HKBPTKQnIay4Fw76bEy8PVxKEDQRKTzs".

## Notes
* `find /` will find every file on the system. 
* To find a file of a particular size, you can use units:
  * b - for 512-byte blocks (this is the default if no suffix is used)
  * c - for bytes
  * w - for two-byte words
  * k - for Kilobytes (units of 1024 bytes)
  * M - for Megabytes (units of 1048576 bytes)
  * G - for Gigabytes (units of 1073741824 bytes)
* We use `2>&1` and `grep` to filter out error messages.
  * File descriptor 1 is the standard output (stdout).
File descriptor 2 is the standard error (stderr). `2>&1` is to redirect stderr to stdout. `&` indicates that what follows and precedes is a file descriptor and not a filename. 
  * `grep` is an acronym that stands for Global Regular Expression Print. The basic synatx is `grep <keyword> <filename>` To print any line from a file that contains a specific keyword. `grep -v "<keyword>"` excludes all lines that contain "\<keyword\>" (`-v` means to invert the search). Use `-i` to ignore case.

