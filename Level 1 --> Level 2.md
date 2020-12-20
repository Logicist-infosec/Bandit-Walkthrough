# Level 1 --> Level 2

> ## Level Goal
> The password for the next level is stored in a file called - located in the home directory
> ## Commands you may need to solve this level
> ls, cd, cat, file, du, find
> ## Helpful Reading Material
> [Google Search for "dashed filename"](https://www.google.com/search?q=dashed+filename)  
> [Advanced Bash-scripting Guide - Chapter 3 - Special Characters](https://tldp.org/LDP/abs/html/special-chars.html)

## Answer
Run `cat < -` or `cat ./-` to get the result "CV1DtqXWVFXTvM2F0k09SHz0YwRINYA9".
## Notes
 \- as an argument refers to STDIN/STDOUT i.e dev/stdin or dev/stdout. So if you want to open this type of file you have to specify the full location of the file such as ./-, or use redirection `cat < -`.

 