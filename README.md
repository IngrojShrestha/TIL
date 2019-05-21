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

##### Search

###### search forward
```
:/<search_term/search_pattern>
```
Press the **n** key to go directly to the next occurrence of the word in backwards. 

###### search backward
```
:?<search_term/search_pattern>

```
Press the **N** key to go directly to the next occurrence of the word in forward. 

**Highlight Search**
```
:set hlsearch
```
**Remove the highlight of the previous search**
```
:nohlsearch
```

### Download a single folder or directory from a GitHub repo 
* [GitZip](http://kinolien.github.io/gitzip/)
* [DownGit](https://minhaskamal.github.io/DownGit/#/home)


