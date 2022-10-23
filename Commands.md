(man man, less filename,find exec->>..pc)

1. whoami
-> display the user name of the system.(1)

1.0 -> echo 

1.1 >,>> (appends) -> redirect the output into some file .(13) Usually used with echo command.

2. man <command>
-> display manual for that command (2). Use mouse to scroll or press space button or down arrow key.
press / and search for a word hit enter to get the result. 'shift +g' end of the file, g start of the file.

3. ls command with some options ad arguments. ls=list
By default, ls lists just one directory. If you name one or more directories on the command line, ls will list each one. The -R (uppercase R) option lists all subdirectories, recursively. That shows you the whole directory tree starting at the current directory
(3)(5)

4. cd=change directory

5. pwd =print working directory

6. mkdir=make directory (4)

7. rmdir=remove directory
when we remove a directory it does not show any output, using -v it shows output. (6) 
-i does interactive mode.(7)


8. touch- change file timestamp

9. open  
open . -> opens current folder (8)

10. mv -> move files/ folders or rename a file/ folder

11. cp -> copy

12. head/tail -> prints the starting/ending number of lines (default 10 lines ) of a file
we can mentioned number of line require. (9,10,11)

13. date

14. cat -> concatenates files and print the standard output.
concatenates multiple files.
(14,15)

15. less -> less command shows the content stored inside a file.

when there are 1000 lines of code and when we type cat is shows all the lines, in less we can see inital lines fitted in terminal and using space we scroll down or move down just like man.

less filename

16. wc -> word count. It counts the word and some inputs. (16,17,18)

1-> line, 2-> words , 12-> number of bytes.

The echo command is slipping in an extra character at the end of your string, test, a new newline character, \n.

So in effect you're counting this: test\n. You can disable this behavior with the -n switch to echo.

17.| -> piping  passing one command output to the another command.
(19)

18. sort -> its case sensitive 'A' < 'a'. use -f to ignore case . (20,21,22,23,24)

Sorting incase of numeric numbers are different is sort based on digits. for numerical sorting use -n. -r to reverse sort. -u for ignoring the sort with duplicates items , prints sort with unique items.

19. uniq -> it reports or omits the repeating lines. (26,25,27,28)

uniq removes first occurences like but if the same value is present in another line one time it won't be removed. So use sort and uniq both.

SO before using uniq sort everything and then use.
-c count occurences,-d shows duplicate items. -u shows unique items.

20. expansion -> matching patterns using * & ?
?-> matches single character 
*-> matches whole character. (29)
{} (30)
shell first expands the thing then executes the command.

21. diff -> compare 2 files and get the differences. (31)

'<' changes not present, '>'changes present.

22. find -> THe find command can be used to find files or folders matching a particular search pattern. It searches recursively. We can use pattern matching for files. '.' means search in current folder
(32,33,34,35)
TO search folder use d. -i to ignore case sensitivity  

find -type f -size +100k -> list all files which has more than 100kb size.
find -type f -mtime +3 -> list files which were edited more than 3 days ago.

While finding the files or directories we can execute the command for each of them.
In the example find all the files while executing command cat to print all the files.
{} -> placeholder, \; -> terminating the executing command. (36)

23. grep -> Global regular expression print. it is use to search in files,logs, or combine it with pipes to filter output of another command.

