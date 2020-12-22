# Level 8 --> Level 9
> ## Level Goal
> The password for the next level is stored in the file data.txt and is the only line of text that occurs only once
>
> ## Commands you may need to solve this level
> grep, sort, uniq, strings, base64, tr, tar, gzip, bzip2, xxd
>
> ## Helpful Reading Material  
> [Piping and Redirection](https://ryanstutorials.net/linuxtutorial/piping.php)

## Answer
Run `sort data.txt | uniq -u` to get the password "UsvVyFSfZZWbi6wgC7dAFyFuR6jQQUhR".

## Notes

### Piping and redirection 
"Normally, we will get our output on the screen, which is convenient most of the time, but sometimes we may wish to save it into a file to keep as a record, feed into another system, or send to someone else." 

* `>` Save output to a file.
* `>>` Append output to a file.
* `<` Read input from a file.
* `2>` Redirect error messages.
* `|` Send the output from one program as input to another program (piping).

### `sort` and `uniq`

"The `uniq` commands expects adjacent lines in inputs. To find unique occurrences where the lines are not adjacent a file needs to be sorted before passing to `uniq`." (see [here](https://shapeshed.com/unix-uniq/#:~:text=To%20find%20unique%20occurrences%20where,txt%20.&text=As%20duplicates%20are%20adjacent%20uniq,the%20result%20to%20standard%20output.))
* `uniq file` No repeated lines in the output.
* `-c` Dispaly number of repetitions for each line.
* `-d` Only print duplicate lines.
* `-u` Only print lines that are not repeated.
