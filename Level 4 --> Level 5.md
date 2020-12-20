# Level 4 → Level 5

> ## Level Goal
>The password for the next level is stored in the only human-readable file in the inhere directory. Tip: if your terminal is messed up, try the “reset” command.
> ## Commands you may need to solve this level
> ls, cd, cat, file, du, find

## Answer
List all files and directories in home directory by running `ls` and then go to directory "inhere" by running `cd inhere`. List the contents in the directory and then check the file type of each file in the directory by running `file ./-*`, then open the ASCII text file `cat ./-file07` to obtain the password "koReBOKuIDDepwhWk7jZC0RTdopnAYKh". 

## Notes
The asterisk `*` represents any number of unknown characters. Use it when searching for documents or files for which you have only partial names.
