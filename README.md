# TIL (Today I Learned)
A minimal repo for my #TIL stuffs related to programming, technology and anything.

--------------
--------------

## November 14, 2017


### 1. Unzip files
#### Unpacking the zip files
```bash
$ unzip <filename>
```

#### Unpacking the .tar and .tar.gz files
```bash
$ tar -xf <filename>
```

#### Unpacking the .gz files
```bash
$ gunzip <filename>
```


### 2. grep commands
grep command handles search patterns called Regular Expression.
#### Find a word in a text file
```bash
$ grep <word> <filename>
```
This command produces all the lines from the text file <filename> that contain the given word <word>.

```bash
$ grep -i <word> <filename>
```
-i ignores the upper and lower case distinction. It provides all the lines containing the word either in uppercase, lowercase or both.

##### Searching multiple words in a text file
```bash
$ egrep 'word1|word2|word3' <filename>
```

### 3. find commands
find command is used to locate specific file by name or extension.
#### Find a file in current and sub-directories.
```bash
$ find . -name <filename>
```

#### Find all .txt files in the /home and sub-directories.
```bash
$ find /home -name *.txt
```

#### Find an empty file within the current directory.
```bash
$ find . -type f -empty
```

### 4. nohup commands

nohup is a POSIX command to ignore the HUP (hangup) signal (wikipedia)

* [Nohup Commands](https://linux.101hacks.com/unix/nohup-command/)
* [Tail commands](https://linuxize.com/post/linux-tail-command/)

Executing python script in background
```bash
$ nohup python script.py > script.log &
```
Watch log file for the changes
```bash
$ tail -f script.log
```

### 5. vi commands
* [Cheat Sheet](http://www.atmos.albany.edu/daes/atmclasses/atm350/vi_cheat_sheet.pdf)
* [Cheat Sheet-II](http://www.cse.scu.edu/~yfang/coen11/vi-CheatSheet.pdf)

```
$ vi +commandHere fileName
$ vi +/searchTermHere fileName
$ vi +/LineNumberHere fileName
```

```
$ vi +/artificial sample.txt
```

##### Shorcuts
|Shorcuts|Description|
| ------------- | ------------- |
|^                                 |Begining of the line
|$                                 |End of the line
|Shift + Arrow(R/L)                |Move the cursor a word forward/backward
|:n                                |Goto Line number **n**
|G                                 |Goto the last line
|:1                                |Goto the first line
|:set number                       |Display line number
|:set nonumber                     |Hide line number
|n                                 |Go directly to the next occurrence of the word in backwards
|N                                 |Go directly to the next occurrence of the word in forwards
|*                                 |Find all occurrences of the word that is under the cursor
|:set mouse=a                      |Enable mouse
|:set mouse-=a                     |Disable mouse
|:set paste                        |Enable paste
|:set nopaste                      |Disable paste
|Ctrl+C/Ctrl+V                     |Copy/Paste
|u                                 |Undo
|r                                 |Redo
|dd                                |Delete the line
|:1,$d                             |Delete all lines
|v                                 |Select from where your cursor is
|V                                 |Select the entire line
|y                                 |Copy selected text
|d                                 |Cut selected text
|P                                 |Paste it before your cursor
|p                                 |Paste it after your cursor
|:set hlsearch                     |Highlight Search
|:nohl search                      |Remove the highlight of the previous search
|:?<search_term/search_pattern>    |Search backward
|:/<search_term/search_pattern>    |Search forward
|:%s/old-string/new-string/        |Replace first occurrence of <old-string> with <new-string> on all lines  
|:s/old-string/new-string/         |Replace first occurrence of <old-string> with <new-string> on current line
|:2,8s/old-string/new-string/      |Replace first occurrence of <old-string> with <new-string> on lines 2 through 8 only
|:.,+100s/foo/bar/                 |Replace first occurrence of foo with bar starting at the current line for the next 100 lines
|:%s/foo/bar/g                     |Replace all occurrences of word foo with bar on all lines, use the g option (which indicates all occurrences on a line).
|:s/foo/bar/g                      |Replace all occurrences of word foo with bar on current line


### Download a single folder or directory from a GitHub repo 
* [GitZip](http://kinolien.github.io/gitzip/)
* [DownGit](https://minhaskamal.github.io/DownGit/#/home)


### File Permissions
* [File Permissions in Linux/Unix](https://www.guru99.com/file-permissions.html)
* [Unix / Linux - File Permission / Access Modes](https://www.tutorialspoint.com/unix/unix-file-permission.htm)

