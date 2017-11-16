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


