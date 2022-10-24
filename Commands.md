# Basic Linux Commands
(man man, less filename,find exec->>..pc)

## echo 

- echo command in linux is used to display line of text/string that are passed as an argument .

- **SYNTAX**: `echo [option] [string]`

- E.g `echo -e "Geeks \bfor \bGeeks"` (it removes all the spaces in between the text)

## touch

- The touch command is a standard command used in UNIX/Linux operating system which is used to create, change and modify timestamps of a file. 
- It is used to create a file without any content. The file created using touch command is empty. This command can be used when the user doesn’t have data to store at the time of file creation.

## whoami

- It displays the username of the current user when this command is invoked.

- **SYNTAX**: `whoami [option]`

![](https://github.com/codophilic/LearnLinux/blob/main/Commands/1.PNG)

## >> Operator

- '>' operator overrides the current content of a file with the output.
- '>>' appends redirect the output into the file along with the original content .

![](https://github.com/codophilic/LearnLinux/blob/main/Commands/13.PNG)

## man 

- display manual for that command. *(Use mouse to scroll or press space button or down arrow key.
press '/' and search for a word hit enter to get the result. 'shift+g' end of the file, 'g' start of the file.)*

![](https://github.com/codophilic/LearnLinux/blob/main/Commands/2.PNG)

## ls 

- ls is a Linux shell command that lists directory contents of files and directories.
- By default, ls lists just one directory. If you name one or more directories on the command line, ls will list each one of those directories.
- The -R (uppercase R) option lists all subdirectories, recursively. That shows you the whole directory tree starting at the current directory
- **SYNTAX**: `ls [option]`
- [ls](https://www.javatpoint.com/linux-ls)

![](https://github.com/codophilic/LearnLinux/blob/main/Commands/3.PNG)
![](https://github.com/codophilic/LearnLinux/blob/main/Commands/5.PNG)

## cd

- cd command in linux known as change directory command. It is used to change current working directory. 

- **SYNTAX**: `cd [directory]`

## pwd 

- `pwd` stands for Print Working Directory. It prints the path of the working directory, starting from the root.

## mkdir

- mkdir command in Linux allows the user to create directories (also referred to as folders in some operating systems).
- This command can create multiple directories at once as well as set the permissions for the directories.
- **SYNTAX**: `mkdir [options...] [directories ...]`

![](https://github.com/codophilic/LearnLinux/blob/main/Commands/4.PNG)

## rmdir

- rmdir command is used remove empty directories from the filesystem in Linux. The rmdir command removes each and every directory specified in the command line only if these directories are empty. 
- So if the specified directory has some directories or files in it then this cannot be removed by rmdir command.
- **SYNTAX**: rmdir [options] [directories…]

- **-v, –verbose**: This option displays verbose information for every directory being processed.

![](https://github.com/codophilic/LearnLinux/blob/main/Commands/6.PNG)

- **-i** does interactive mode.
![](https://github.com/codophilic/LearnLinux/blob/main/Commands/7.PNG)


## open  

- opens current folder or file

![](https://github.com/codophilic/LearnLinux/blob/main/Commands/8.PNG)

## mv

- Use the mv command to move files and directories from one directory to another or to rename a file or directory. 
- This command normally works silently means no prompt for confirmation. 

- **SYNTAX**: `mv [Option] source destination`

## cp 

- cp stands for copy. This command is used to copy files or group of files or directory. It creates an exact image of a file on a disk with different file name. cp command require at least two filenames in its arguments.

- **SYNTAX**:

`cp [OPTION] Source Destination

cp [OPTION] Source Directory

cp [OPTION] Source-1 Source-2 Source-3 Source-n Directory`

- First and second syntax is used to copy Source file to Destination file or Directory.
Third syntax is used to copy multiple Sources(files) to Directory.


## head

- The head command, as the name implies, print the top N number of data of the given input. By default, it prints the first 10 lines of the specified files. 
- If more than one file name is provided then data from each file is preceded by its file name.  
- **SYNTAX**: `head [OPTION]... [FILE]...`

![](https://github.com/codophilic/LearnLinux/blob/main/Commands/9.PNG)
![](https://github.com/codophilic/LearnLinux/blob/main/Commands/10.PNG)
![](https://github.com/codophilic/LearnLinux/blob/main/Commands/11.PNG)

## tail

- It is the complementary of head command.The tail command, as the name implies, print the last N number of data of the given input. By default it prints the last 10 lines of the specified files. 
- If more than one file name is provided then data from each file is precedes by its file name.
- **SYNTAX**: `tail [OPTION]... [FILE]...`


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

grep [options] pattern [files]

https://www.geeksforgeeks.org/grep-command-in-unixlinux/

24. du -> disk usage. Gives the size of directories. (37,38)du -h gives human readable format.

25. df -> disk free provides information about file system shows disk utilization with space left and allocated etc. (39)

26. history -> list all the commands ran in the past. TO run a past command we can use its ID number.
!(number) (40)

27. ps -> process status. (41,42)
ps ax shows process initiated by any users on the system.

28. top-> The top (table of processes) command shows a real-time view of running processes in Linux and displays kernel-managed tasks. The command also provides a system information summary that shows resource utilization, including CPU and memory usage.

https://phoenixnap.com/kb/top-command-in-linux#:~:text=The%20top%20(table%20of%20processes,including%20CPU%20and%20memory%20usage.

29. kill -> linux process receiev signals and react to them. The kill program can send a variety of signals.
kill <PID>

30. alias -> In Linux, an alias is a shortcut that references a command. An alias replaces a string that invokes a command in the Linux shell with another user-defined string. Aliases are mostly used to replace long commands, improving efficiency and avoiding potential spelling errors. (43,44)
It is not permanent , if will kill the terminal its no longer supported.

now to make it permanent we need to place it in a file depending on the shell like for bash we will add the alias in .basharc file.

31. xargs -> xargs command is used to convert input from standard input into arguments to a command. Through xargs the output of a command is used as the input of another command.

command1 | xargs command2

Xargs is a great command that reads streams of data from standard input, then generates and executes command lines; meaning it can take output of a command and passes it as argument of another command. If no command is specified, xargs executes echo by default. You many also instruct it to read data from a file instead of stdin.

let say there are multiple files in a folder and some files needs to be deleted. Those deletion of file name is present in a deletefile.txt file. So to pass the content of deletefile.txt as an argument to remove command.
We cannot use cat deletefile.txt | rm -> since it shows one single content to remove command.
So we need to split into arguments of deadfile and pass those arguments to the remove command. (45)

Using xargs & | it converts the output of one command into arguments and pass it to another command.(46)

32. ln -> It is used to create links. Its like a pointer to another file just like windows shortcuts.

There are two types of hard links and soft links.

Hard links -> You can't link directories and cannot link external filesystem (disk)
let say if we want two files to be sync not copy its pointing to the same file. we can use hard links.

ln original newlink (47)

if we delete any one of the file the other file persists.
https://www.geeksforgeeks.org/soft-hard-links-unixlinux/

soft links-> are same as hard links but when original file is deleted the another file linked also gets deleted.

33. who -> displays the users logged in the system. when a server is used by multiple people we can see which user logged in at what time.

34. passwd -> One can changed the password of the linux system.