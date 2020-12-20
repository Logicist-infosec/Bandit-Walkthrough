# Level 3 → Level 4

> ## Level Goal
>The password for the next level is stored in a hidden file in the inhere directory.
> ## Commands you may need to solve this level
>ls, cd, cat, file, du, find

## Answer
1. Use `ls -a` to list all files and directories even if they are hidden. 
2. `cd inhere` to open directory "inhere".
3. `cat .hidden` to open the hidden file and get result "pIwrPrtPN36QITSp3EQaw936yaFoFgAB".

## Notes
Symbol `.` before the filename and directory name is used to indicate that file or directory is hidden. 