# Level 0 --> Level 1

> ## Level Goal
> The password for the next level is stored in a file called readme located in the home directory. Use this password to log into bandit1 using SSH. Whenever you find a password for a level, use SSH (on port 2220) to log into that level and continue the game.
> 
> ## Commands you may need to solve this level
> ls, cd, cat, file, du, find

## Answer
1. After login into the bandit server by SSH, run command `ls` to list the files and directories in home directory. A file named "readme" is listed.
2. Run `cat readme` to open the file and get the password "boJ9jbbUNNfktd78OOpsqOltutMc3MY1".

## Notes
1. Command `file <filename>` could show type of the file. 
2. Command `find <filename>` is used to find a specific file.
3. Other commands used to open a text file include: `more`, `less`.


