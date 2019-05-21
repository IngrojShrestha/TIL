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
|$                                 |Begining of the line
|^                                 |End of the line
|:n                                |Goto Line number **n**
|G                                 |Goto the last line
|:1                                |Goto the first line

|:set number                       |Display line number

|:set nonumber                     |Hide line number
|:set hlsearch                     |Highlight Search
|:nohl search                      |Remove the highlight of the previous search

|:?<search_term/search_pattern>    |Search backward
|:/<search_term/search_pattern>    |Search forward

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

|v                                 |Select from where your cursor is
|V                                 |Select the entire line
|y                                 |Copy selected text
|d                                 |Cut selected text
|P                                 |Paste it before your cursor
|p                                 |Paste it after your cursor



### Download a single folder or directory from a GitHub repo 
* [GitZip](http://kinolien.github.io/gitzip/)
* [DownGit](https://minhaskamal.github.io/DownGit/#/home)

