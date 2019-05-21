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

```
$ vi +commandHere fileName
$ vi +/searchTermHere fileName
$ vi +/LineNumberHere fileName
```

```
$ vi +/artificial sample.txt
```

### Download a single folder or directory from a GitHub repo 
* [GitZip](http://kinolien.github.io/gitzip/)
* [DownGit](https://minhaskamal.github.io/DownGit/#/home)


