# Basic Linux Commands
(man man, less filename,find exec->>..pc)

## echo 

- echo command in linux is used to display line of text/string that are passed as an argument .
- **SYNTAX**: `echo [option] [string]`
- E.g `echo -e "Geeks \bfor \bGeeks"` (it removes all the spaces in between the text)
- **The echo command adds an extra character at the end of a string which is a new newline character *\n*.**
- Disable this behavior with the **-n** switch to `echo`. E.g `echo -n "Hello Linux"`.

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

- display manual for that command.
- **Enter key**: to scroll down line by line.
- **Space bar**: To go to the next page.
- **press b key**: To go to back one page.
- Use the mouse scroll wheel, the up and down arrow keys, or the PgDn and PgUp keys to navigate through it.
- Use /{word}+enter to find a particular word

![](https://github.com/codophilic/LearnLinux/blob/main/Commands/2.PNG)

## ls 

- ls is a Linux shell command that lists directory contents of files and directories.
- By default, ls lists just one directory. If you name one or more directories on the command line, ls will list each one of those directories.
- The -R (uppercase R) option lists all subdirectories, recursively. That shows you the whole directory tree starting at the current directory
- **SYNTAX**: `ls [option]`
- [learn more about ls](https://www.javatpoint.com/linux-ls)

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


## tail

- It is the complementary of head command.The tail command, as the name implies, print the last N number of data of the given input. By default it prints the last 10 lines of the specified files. 
- If more than one file name is provided then data from each file is precedes by its file name.
- **SYNTAX**: `tail [OPTION]... [FILE]...`

![](https://github.com/codophilic/LearnLinux/blob/main/Commands/11.PNG)


## date

- date command is used to display the system date and time. date command is also used to set date and time of the system. 
- By default the date command displays the date in the time zone on which unix/linux operating system is configured.You must be the super-user (root) to change the date and time.
- **SYNTAX**: `date [OPTION]... [+FORMAT]`
- [learn more about date](https://www.geeksforgeeks.org/date-command-linux-examples/)

![](https://github.com/codophilic/LearnLinux/blob/main/Commands/12.PNG)

## cat 

- Cat(concatenate) command is very frequently used in Linux. It reads data from the file and gives their content as output. It helps us to create, view, concatenate files. So let us see some frequently used cat commands. 

![](https://github.com/codophilic/LearnLinux/blob/main/Commands/13.PNG)
![](https://github.com/codophilic/LearnLinux/blob/main/Commands/14.PNG)
![](https://github.com/codophilic/LearnLinux/blob/main/Commands/15.PNG)

## less 

- Less command is a Linux utility that can be used to read the contents of a text file one page(one screen) at a time. It has faster access because if file is large it doesn’t access the complete file, but accesses it page by page.
- **SYNTAX**: `less file_name`
- [Learn more about less](https://www.geeksforgeeks.org/less-command-linux-examples/)

## wc 

- WC stands for word count. As the name implies, it is mainly used for counting purpose.
-It is used to find out number of lines, word count, byte and characters count in the files specified in the file arguments.
-By default it displays four-columnar output.
-First column shows number of lines present in a file specified, second column shows number of words present in the file, third column shows number of characters present in file and fourth column itself is the file name which are given as argument.

![](https://github.com/codophilic/LearnLinux/blob/main/Commands/16.PNG)
![](https://github.com/codophilic/LearnLinux/blob/main/Commands/17.PNG)
![](https://github.com/codophilic/LearnLinux/blob/main/Commands/18.PNG)

*(The echo command adds an extra character at the end of a string which is a new newline character \n.Disable this behavior with the **-n** switch to `echo`. E.g `echo -n "Hello Linux"`.)*

## pipe(|) 

- Pipe is used to combine two or more commands, and in this, the output of one command acts as input to another command, and this command’s output may act as input to the next command and so on.
- **Pipes are unidirectional i.e data flows from left to right through the pipeline**
- **SYNTAX**: `command_1 | command_2 | command_3 | .... | command_N`

![](https://github.com/codophilic/LearnLinux/blob/main/Commands/19.PNG)


## sort 

- SORT command is used to sort a file, arranging the records in a particular order. By default, the sort command sorts file assuming the contents are ASCII. *('A' < 'a', use **-f** to ignore case )*
- Using options in the sort command can also be used to sort numerically. 
- Incase of numeric numbers sorting is done based on digits. For numerical sorting use **-n**. 
- Use **-r** to reverse sort. Use **-u** for printing unique items.

![](https://github.com/codophilic/LearnLinux/blob/main/Commands/20.PNG)
![](https://github.com/codophilic/LearnLinux/blob/main/Commands/21.PNG)
![](https://github.com/codophilic/LearnLinux/blob/main/Commands/22.PNG)
![](https://github.com/codophilic/LearnLinux/blob/main/Commands/23.PNG)
![](https://github.com/codophilic/LearnLinux/blob/main/Commands/24.PNG)

## uniq 

- uniq is the tool that helps to detect the adjacent duplicate lines and also deletes the duplicate lines. uniq filters out the adjacent matching lines from the input file (that is required as an argument) and writes the filtered data to the output file. 
- Use **uniq** and **sort** to remove duplocate items.
- Use **-c** to get count occurences,**-d** shows duplicate items & **-u** shows unique items.

![](https://github.com/codophilic/LearnLinux/blob/main/Commands/26.PNG)
![](https://github.com/codophilic/LearnLinux/blob/main/Commands/25.PNG)
![](https://github.com/codophilic/LearnLinux/blob/main/Commands/27.PNG)
![](https://github.com/codophilic/LearnLinux/blob/main/Commands/28.PNG)


## Wildcards 

- Wildcards are also often referred to as glob patterns (or when using them, as "globbing").
- [Learn more about it here](https://www.linuxjournal.com/content/pattern-matching-bash)

![](https://github.com/codophilic/LearnLinux/blob/main/Commands/29.PNG)
![](https://github.com/codophilic/LearnLinux/blob/main/Commands/30.PNG)

- Shell first expands the thing {} then executes the command.

## diff 

- diff stands for difference. This command is used to display the differences in the files by comparing the files line by line. 
- The important thing to remember is that diff uses certain special symbols and instructions that are required to make two files identical. It tells you the instructions on how to change the first file to make it match the second file. 
- Special symbols are: 
a : add
c : change
d : delete
- **SYNTAX**: `diff [options] File1 File2 `
- [Learn more about diff](https://www.geeksforgeeks.org/diff-command-linux-examples/)

![](https://github.com/codophilic/LearnLinux/blob/main/Commands/31.PNG)


## find 

- It can be used to find files and directories and perform subsequent operations on them. It supports searching by file, wildcards, folder, name, creation date, modification date, owner and permissions. 
- **SYNTAX**: `find [where to start searching from]
 [expression determines what to find] [-options] [what to find]`

![](https://github.com/codophilic/LearnLinux/blob/main/Commands/32.PNG)
![](https://github.com/codophilic/LearnLinux/blob/main/Commands/33.PNG)
![](https://github.com/codophilic/LearnLinux/blob/main/Commands/34.PNG)
![](https://github.com/codophilic/LearnLinux/blob/main/Commands/35.PNG)

- Search folder use **d**. Use **-i** to ignore case sensitivity  

- E.g `find -type f -size +100k` (list all files which has more than 100kb size).
`find -type f -mtime +3` (list files which were edited more than 3 days ago).

- While finding the files or directories we can execute the command for each of them.
- In the example find all the files while executing command cat to print all the files.
**{} -> placeholder, \; -> terminating the executing command**. 

![](https://github.com/codophilic/LearnLinux/blob/main/Commands/36.PNG)

## grep 

- Global regular expression print. it is use to search in files,logs, or combine it with pipes to filter output of another command.
- **SYNTAX**: grep [options] pattern [files]
- [Learn more about grep](https://www.geeksforgeeks.org/grep-command-in-unixlinux/)

## du 

- du command, short for disk usage, is used to estimate file space usage.
- The du command can be used to track the files and directories which are consuming excessive amount of space on hard disk drive. 
- **SYNTAX**: `du [OPTION]... [FILE]...`
- `du -h` gives human readable format.

![](https://github.com/codophilic/LearnLinux/blob/main/Commands/37.PNG)
![](https://github.com/codophilic/LearnLinux/blob/main/Commands/38.PNG)

## df 

- disk free provides information about file system shows disk utilization with space left and allocated etc.

![](https://github.com/codophilic/LearnLinux/blob/main/Commands/39.PNG)

## history 

- list all the commands ran in the past. To run a past command we can use its ID number and run it by `!(number)`.

![](https://github.com/codophilic/LearnLinux/blob/main/Commands/40.PNG)

## ps 

- process status. 
- `ps ax` shows process initiated by any users on the system.

![](https://github.com/codophilic/LearnLinux/blob/main/Commands/41.PNG)
![](https://github.com/codophilic/LearnLinux/blob/main/Commands/42.PNG)

## top

- The top (table of processes) command shows a real-time view of running processes in Linux and displays kernel-managed tasks. The command also provides a system information summary that shows resource utilization, including CPU and memory usage.
- [Seehere](https://phoenixnap.com/kb/top-command-in-linux#:~:text=The%20top%20(table%20of%20processes,including%20CPU%20and%20memory%20usage)

## kill 

- linux process receive signals and react to them. The kill program can send a variety of signals.
- **SYNTAX**: `kill <PID>`

## alias 

- In Linux, an alias is a shortcut that references a command. An alias replaces a string that invokes a command in the Linux shell with another user-defined string. Aliases are mostly used to replace long commands, improving efficiency and avoiding potential spelling errors. 

![](https://github.com/codophilic/LearnLinux/blob/main/Commands/43.PNG)
![](https://github.com/codophilic/LearnLinux/blob/main/Commands/44.PNG)

- It is not permanent , if will kill the terminal its no longer supported.

- Now to make it permanent we need to place it in a file depending on the shell like for bash we will add the alias in .basharc file.

## xargs 

- xargs command is used to convert input from standard input into arguments to a command. Through xargs the output of a command is used as the input of another command.
- **SYNTAX**: `command1 | xargs command2`
- Xargs is a great command that reads streams of data from standard input, then generates and executes command lines; meaning it can take output of a command and passes it as argument of another command. If no command is specified, xargs executes echo by default. You many also instruct it to read data from a file instead of stdin.
- let say there are multiple files in a folder and some files needs to be deleted. Those deletion of file name is present in a **deletefile.txt** file. So to pass the content of **deletefile.txt** as an argument to remove command.
We cannot use `cat deletefile.txt | rm` *(since it shows one single content to remove command)*.
- So we need to split into arguments of deadfile and pass those arguments to the remove command. 

![](https://github.com/codophilic/LearnLinux/blob/main/Commands/45.PNG)
![](https://github.com/codophilic/LearnLinux/blob/main/Commands/46.PNG)

- Using **xargs** & **pipe(|)** it converts the output of one command into arguments and pass it to another command.

## ln 

- It is used to create links. Its like a pointer to another file just like windows shortcuts.
- There are two types of **hard links** and **soft links**.
1. Hard links: You can't link directories and cannot link external filesystem (disk)
let say if we want two files to be sync not copy its pointing to the same file. we can use hard links.

**SYNTAX**: `ln original newlink` 

![](https://github.com/codophilic/LearnLinux/blob/main/Commands/47.PNG)

- if we delete any one of the file the other file persists. [Check here](https://www.geeksforgeeks.org/soft-hard-links-unixlinux/)

2. soft links: are same as hard links but when original file is deleted the another file linked also gets deleted.

## who 

- Displays the users logged in the system. when a server is used by multiple people we can see which user logged in at what time.

## passwd 

- One can changed the password of the linux system.