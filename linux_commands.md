# Basic Linux Commands

# Dheeraj Lalwani
## Roll Number: 1902085
## 18/02/2021


<br>

<hr>

<br>

# 1] `ls`



```
masterx@Dheeraj:~$ ls
annoyingAssignments  data.txt        hell.sh     timepass2.sh
cooltext.txt         documents       lame.txt    timepass3.sh
data2.txt            ftrax           music       timepass.sh
data3.txt            greaterthan.sh  resume.pdf  videos
masterx@Dheeraj:~$
```



```
Usage: ls [OPTION]... [FILE]...
List information about the FILEs (the current directory by default).
Sort entries alphabetically if none of -cftuvSUX nor --sort is specified.

This will list all the non hidden files and folders in CWD (Current working directory)
```


## 1.1] `ls -a` or `ls --all` 

### do not ignore entries starting with a  `"."` 


```
masterx@Dheeraj:~$ ls -a
.                    data.txt        music
..                   documents       .profile
annoyingAssignments  .emacs.d        .python_history
.bash_history        ftrax           resume.pdf
.bash_logout         .git            timepass2.sh
.bashrc              .gitconfig      timepass3.sh
.cache               greaterthan.sh  timepass.sh
cooltext.txt         hell.sh         videos
data2.txt            lame.txt        .vscode-server
data3.txt            .local          .wget-hsts
masterx@Dheeraj:~$
```



## 1.2] `ls -v`

### Lists the files in a naturally sorted manner instead of lexicographically 

<br>

### `ls` (without -v) 


```
masterx@Dheeraj:~/annoyingAssignments$ ls
test_file10.txt  test_file18.txt  test_file25.txt  test_file32.txt  test_file3.txt   test_file47.txt  test_file8.txt
test_file11.txt  test_file19.txt  test_file26.txt  test_file33.txt  test_file40.txt  test_file48.txt  test_file9.txt
test_file12.txt  test_file1.txt   test_file27.txt  test_file34.txt  test_file41.txt  test_file49.txt
test_file13.txt  test_file20.txt  test_file28.txt  test_file35.txt  test_file42.txt  test_file4.txt
test_file14.txt  test_file21.txt  test_file29.txt  test_file36.txt  test_file43.txt  test_file50.txt
test_file15.txt  test_file22.txt  test_file2.txt   test_file37.txt  test_file44.txt  test_file5.txt
test_file16.txt  test_file23.txt  test_file30.txt  test_file38.txt  test_file45.txt  test_file6.txt
test_file17.txt  test_file24.txt  test_file31.txt  test_file39.txt  test_file46.txt  test_file7.txt
```


### `ls -v`

```
masterx@Dheeraj:~/annoyingAssignments$ ls -v
test_file1.txt  test_file9.txt   test_file17.txt  test_file25.txt  test_file33.txt  test_file41.txt  test_file49.txt
test_file2.txt  test_file10.txt  test_file18.txt  test_file26.txt  test_file34.txt  test_file42.txt  test_file50.txt
test_file3.txt  test_file11.txt  test_file19.txt  test_file27.txt  test_file35.txt  test_file43.txt
test_file4.txt  test_file12.txt  test_file20.txt  test_file28.txt  test_file36.txt  test_file44.txt
test_file5.txt  test_file13.txt  test_file21.txt  test_file29.txt  test_file37.txt  test_file45.txt
test_file6.txt  test_file14.txt  test_file22.txt  test_file30.txt  test_file38.txt  test_file46.txt
test_file7.txt  test_file15.txt  test_file23.txt  test_file31.txt  test_file39.txt  test_file47.txt
test_file8.txt  test_file16.txt  test_file24.txt  test_file32.txt  test_file40.txt  test_file48.txt
```


## 1.3] `ls -l`
### use a long listing format to list all files and folder 
 

```
masterx@Dheeraj:~$ ls -l
total 60
drwxr-xr-x 3 masterx masterx 4096 Feb 24 20:34 boringAssingments
-rw-r--r-- 1 masterx masterx   18 Feb 18 13:46 cooltext.txt
-rw-r--r-- 1 masterx masterx   11 Feb 18 13:27 data2.txt
-rw-rw-r-- 1 masterx masterx   13 Feb 18 13:33 data3.txt
-rwxrwxrwx 1 masterx masterx   20 Feb 18 13:09 data.txt
drwxr-xr-x 2 masterx masterx 4096 Feb 13 17:56 documents
drwxr-xr-x 2 masterx masterx 4096 Feb 13 17:55 ftrax
-rw-r--r-- 1 masterx masterx   98 Feb 18 14:13 greaterthan.sh
-rw-r--r-- 1 masterx masterx   79 Feb 18 14:08 hell.sh
-rw-r--r-- 1 masterx masterx   16 Feb 14 02:25 lame.txt
drwxr-xr-x 2 masterx masterx 4096 Feb 13 17:56 music
-rw-r--r-- 1 masterx masterx    0 Feb 13 17:57 resume.pdf
-rw-r--r-- 1 masterx masterx   53 Feb 18 14:03 timepass2.sh
-rw-r--r-- 1 masterx masterx  104 Feb 18 14:05 timepass3.sh
-rw-r--r-- 1 masterx masterx   52 Feb 18 14:02 timepass.sh
drwxr-xr-x 2 masterx masterx 4096 Feb 13 17:57 videos
masterx@Dheeraj:~$
```




<br>
<hr>
<br>

# 2] `mkdir`



```
masterx@Dheeraj:~$ ls
cooltext.txt  documents       lame.txt      timepass3.sh
data2.txt     ftrax           music         timepass.sh
data3.txt     greaterthan.sh  resume.pdf    videos
data.txt      hell.sh         timepass2.sh
masterx@Dheeraj:~$ mkdir boringAssingments
masterx@Dheeraj:~$ ls
boringAssingments  data.txt        hell.sh     timepass2.sh
cooltext.txt       documents       lame.txt    timepass3.sh
data2.txt          ftrax           music       timepass.sh
data3.txt          greaterthan.sh  resume.pdf  videos
masterx@Dheeraj:~$
```

```
Usage: mkdir [OPTION]... DIRECTORY...
Create the DIRECTORY(ies), if they do not already exist.
```


## 2.1] `mkdir path/which/you/want -p` or `mkdir path/which/you/want --parent`

### Will give no error if existing and make parent directories as needed


```
masterx@Dheeraj:~/boringAssingments$ ls
masterx@Dheeraj:~/boringAssingments$ mkdir OS/Assignment_1
mkdir: cannot create directory ‘OS/Assignment_1’: No such file or directory
masterx@Dheeraj:~/boringAssingments$ mkdir OS/Assignment_1 -p
masterx@Dheeraj:~/boringAssingments$ ls
OS
masterx@Dheeraj:~/boringAssingments$ cd OS/
masterx@Dheeraj:~/boringAssingments/OS$ ls
Assignment_1
```








## 2.2] `mkdir dirName -v` or `mkdir dirName --version`

### print a message for each created directory

```
masterx@Dheeraj:~$ ls
boringAssingments  data3.txt  ftrax           lame.txt    timepass2.sh  videos
cooltext.txt       data.txt   greaterthan.sh  music       timepass3.sh
data2.txt          documents  hell.sh         resume.pdf  timepass.sh
masterx@Dheeraj:~$ mkdir project -v
mkdir: created directory 'project'
masterx@Dheeraj:~$ ls
boringAssingments  data3.txt  ftrax           lame.txt  resume.pdf    timepass.sh
cooltext.txt       data.txt   greaterthan.sh  music     timepass2.sh  videos
data2.txt          documents  hell.sh         project   timepass3.sh
masterx@Dheeraj:~$
```


## 2.3] `mkdir -m `

### Sets mode like in chmod

```
masterx@Dheeraj:~$ mkdir -m 0022 newModeDirectory
masterx@Dheeraj:~$ ls
folder1   folder11  folder13  folder15  folder3  folder5  folder7  folder9
folder10  folder12  folder14  folder2   folder4  folder6  folder8  newModeDirectory
masterx@Dheeraj:~$ ls -l
total 64
drwxr-xr-x 2 masterx masterx 4096 Feb 14 21:38 folder1
drwxr-xr-x 2 masterx masterx 4096 Feb 14 21:38 folder10
drwxr-xr-x 2 masterx masterx 4096 Feb 14 21:38 folder11
drwxr-xr-x 2 masterx masterx 4096 Feb 14 21:38 folder12
drwxr-xr-x 2 masterx masterx 4096 Feb 14 21:38 folder13
drwxr-xr-x 2 masterx masterx 4096 Feb 14 21:38 folder14
drwxr-xr-x 2 masterx masterx 4096 Feb 14 21:38 folder15
drwxr-xr-x 2 masterx masterx 4096 Feb 14 21:38 folder2
drwxr-xr-x 2 masterx masterx 4096 Feb 14 21:38 folder3
drwxr-xr-x 2 masterx masterx 4096 Feb 14 21:38 folder4
drwxr-xr-x 2 masterx masterx 4096 Feb 14 21:38 folder5
drwxr-xr-x 2 masterx masterx 4096 Feb 14 21:38 folder6
drwxr-xr-x 2 masterx masterx 4096 Feb 14 21:38 folder7
drwxr-xr-x 2 masterx masterx 4096 Feb 14 21:38 folder8
drwxr-xr-x 2 masterx masterx 4096 Feb 14 21:38 folder9
d----w--w- 2 masterx masterx 4096 Feb 25 03:42 newModeDirectory
masterx@Dheeraj:~$
```


<br>
<hr>
<br>



# 3] `chdir` or `cd`

## This command helps us change the current working directory

```
masterx@Dheeraj:~/boringAssingments$ cd ../ftrax
masterx@Dheeraj:~/ftrax$
```





<br>


# 4] `rmdir`

```
masterx@Dheeraj:~$ ls
boringAssingments  data3.txt  ftrax           lame.txt  resume.pdf    timepass.sh
cooltext.txt       data.txt   greaterthan.sh  music     timepass2.sh  videos
data2.txt          documents  hell.sh         project   timepass3.sh
masterx@Dheeraj:~$ rmdir project/
masterx@Dheeraj:~$ ls
boringAssingments  data3.txt  ftrax           lame.txt    timepass2.sh  videos
cooltext.txt       data.txt   greaterthan.sh  music       timepass3.sh
data2.txt          documents  hell.sh         resume.pdf  timepass.sh
masterx@Dheeraj:~$
```


```
Usage: rmdir [OPTION]... DIRECTORY...
Remove the DIRECTORY(ies), if they are empty.
```

## 4.1] `rmdir -p` or `rmdir --parents`

### This command will remove the parent directories also

```
masterx@Dheeraj:~$ rmdir documents/doc1/folder1 -p
masterx@Dheeraj:~$ ls
boringAssingments  data3.txt  greaterthan.sh  music         timepass3.sh
cooltext.txt       data.txt   hell.sh         resume.pdf    timepass.sh
data2.txt          ftrax      lame.txt        timepass2.sh  videos
masterx@Dheeraj:~$
```

## 4.2] `rmdir -v`

### This command output a diagnostic for every directory processed

```
masterx@Dheeraj:~/boringAssingments$ rmdir OS/Assignment_1 -v
rmdir: removing directory, 'OS/Assignment_1'
masterx@Dheeraj:~/boringAssingments$ cd OS/
masterx@Dheeraj:~/boringAssingments/OS$ ls
masterx@Dheeraj:~/boringAssingments/OS$
```


<br>
<hr>
<br>


# 5] `cat` 

```
masterx@Dheeraj:~/boringAssingments/OS$ cat >> newfile.txt
This is new file!
Welcome to my new file.

I think this is a new file.


New files are awesome. Happy new files
        Byee. Regards - newfile.txt

masterx@Dheeraj:~/boringAssingments/OS$ cat newfile.txt
This is new file!
Welcome to my new file.

I think this is a new file.


New files are awesome. Happy new files
        Byee. Regards - newfile.txt
masterx@Dheeraj:~/boringAssingments/OS$
```



```
Usage: cat [OPTION]... [FILE]...
Concatenate FILE(s) to standard output.
```

## 5.1] `cat filename -b`

### This command will number each non empty files

```
masterx@Dheeraj:~/boringAssingments/OS$ cat -b newfile.txt
     1  This is new file!
     2  Welcome to my new file.

     3  I think this is a new file.


     4  New files are awesome. Happy new files
     5          Byee. Regards - newfile.txt
masterx@Dheeraj:~/boringAssingments/OS$
```


## 5.2] `cat filename -E`

### This command will show a `$` at end of each line

```
masterx@Dheeraj:~/boringAssingments/OS$ cat -E newfile.txt
This is new file!$
Welcome to my new file.$
$
I think this is a new file.$
$
$
New files are awesome. Happy new files$
        Byee. Regards - newfile.txt$
masterx@Dheeraj:~/boringAssingments/OS$
```

## 5.3] `cat filename -n`

### This command will number each new line regardless of it being empty or now

```
masterx@Dheeraj:~/boringAssingments/OS$ cat -n newfile.txt
     1  This is new file!
     2  Welcome to my new file.
     3
     4  I think this is a new file.
     5
     6
     7  New files are awesome. Happy new files
     8          Byee. Regards - newfile.txt
masterx@Dheeraj:~/boringAssingments/OS$
```


<br>
<hr>
<br>

# 6] `rm`

```
masterx@Dheeraj:~$ rm data2.txt
masterx@Dheeraj:~$ ls
boringAssingments  data.txt        hell.sh   resume.pdf    timepass.sh
cooltext.txt       ftrax           lame.txt  timepass2.sh  videos
data3.txt          greaterthan.sh  music     timepass3.sh
masterx@Dheeraj:~$
```

```
Usage: rm [OPTION]... [FILE]...
Remove (unlink) the FILE(s).
```

## 6.1] `rm filename -i`

### This command will prompt before every removal


```
masterx@Dheeraj:~$ ls
boringAssingments  ftrax           music         timepass.sh
cooltext.txt       greaterthan.sh  timepass2.sh  videos
data.txt           hell.sh         timepass3.sh
masterx@Dheeraj:~$ rm timepass2.sh timepass3.sh timepass.sh -i
rm: remove regular file 'timepass2.sh'? y
rm: remove regular file 'timepass3.sh'? y
rm: remove regular file 'timepass.sh'? y
masterx@Dheeraj:~$ ls
boringAssingments  data.txt  greaterthan.sh  music
cooltext.txt       ftrax     hell.sh         videos
masterx@Dheeraj:~$
```

## 6.2] `rm -d`

### This command will remove all empty directories

```
masterx@Dheeraj:~$ mkdir music
masterx@Dheeraj:~$ cd music/
masterx@Dheeraj:~/music$ ls
masterx@Dheeraj:~/music$ cd ..
masterx@Dheeraj:~$ rm -d music/
masterx@Dheeraj:~$ ls
boringAssingments  data.txt  greaterthan.sh  videos
cooltext.txt       ftrax     hell.sh
masterx@Dheeraj:~$
```


## 6.3] `rm -v`

### This command will explain what is happening

```
masterx@Dheeraj:~$ ls
boringAssingments  data.txt  greaterthan.sh  videos
cooltext.txt       ftrax     hell.sh
masterx@Dheeraj:~$ rm -v hell.sh greaterthan.sh
removed 'hell.sh'
removed 'greaterthan.sh'
masterx@Dheeraj:~$ ls
boringAssingments  cooltext.txt  data.txt  ftrax  videos
masterx@Dheeraj:~$
```


<br>
<hr>
<br>

# 7] `mv`


```
masterx@Dheeraj:~$ ls
boringAssingments  cooltext.txt  data.txt  ftrax  videos
masterx@Dheeraj:~$ cd videos/
masterx@Dheeraj:~/videos$ ls
masterx@Dheeraj:~/videos$ cd ..
masterx@Dheeraj:~$ mv ftrax videos
masterx@Dheeraj:~$ ls
boringAssingments  cooltext.txt  data.txt  videos
masterx@Dheeraj:~$ cd videos/
masterx@Dheeraj:~/videos$ ls
ftrax
masterx@Dheeraj:~/videos$
```

```
Usage: mv [OPTION]... [-T] SOURCE DEST
  or:  mv [OPTION]... SOURCE... DIRECTORY
  or:  mv [OPTION]... -t DIRECTORY SOURCE...
Rename SOURCE to DEST, or move SOURCE(s) to DIRECTORY.

This command helps us move files, folders and also rename them
```

## 7.1] `mv -i`

### This command will prompt you before overwriting files

```
masterx@Dheeraj:~$ ls
boringAssingments  data.txt  videos
masterx@Dheeraj:~$ cd videos/ftrax/
masterx@Dheeraj:~/videos/ftrax$ ls
cooltext.txt
masterx@Dheeraj:~/videos/ftrax$ cat cooltext.txt
This is cool text 2
masterx@Dheeraj:~/videos/ftrax$ cd ../..
masterx@Dheeraj:~$ cat >> cooltext.txt
This is new cool text
masterx@Dheeraj:~$ mv cooltext.txt videos/ftrax -i
mv: overwrite 'videos/ftrax/cooltext.txt'? y
masterx@Dheeraj:~$ cat videos/ftrax/cooltext.txt
This is new cool text
```

# 7.2] `mv -n`

### This command will not allow overriding of files

```
masterx@Dheeraj:~$ cat >> cooltext.txt
Hello again to new cool test.
^C
masterx@Dheeraj:~$
masterx@Dheeraj:~$ cat >> cooltext.txt
Hello again to new cool test.
^C
masterx@Dheeraj:~$
```

## 7.3]  `mv -v`

### This command will explain what is being done

```
masterx@Dheeraj:~/videos$ mv -v ftrax ../
renamed 'ftrax' -> '../ftrax'
masterx@Dheeraj:~/videos$ ls
masterx@Dheeraj:~/videos$ cd ..
masterx@Dheeraj:~$ ls
boringAssingments  cooltext.txt  data.txt  ftrax  videos
masterx@Dheeraj:~$
```


<br>
<hr>
<br>

# 8] `cp`



```
masterx@Dheeraj:~$ cat cooltext.txt
Hello again to new cool test.
masterx@Dheeraj:~$ cat cooltext2.txt
This is cool text 2
masterx@Dheeraj:~$ cp cooltext.txt cooltext2.txt
masterx@Dheeraj:~$ cat cooltext.txt
Hello again to new cool test.
masterx@Dheeraj:~$ cat cooltext2.txt
This is cool text 2
masterx@Dheeraj:~$ cp cooltext.txt cooltext2.txt
```

```
Usage: cp [OPTION]... [-T] SOURCE DEST
  or:  cp [OPTION]... SOURCE... DIRECTORY
  or:  cp [OPTION]... -t DIRECTORY SOURCE...
Copy SOURCE to DEST, or multiple SOURCE(s) to DIRECTORY.
```




## 8.1] `cp -i`

### This command will prompt before overwriting the file

```
masterx@Dheeraj:~$ cat cooltext.txt
Hello again to new cool test.
This is cool text 1
masterx@Dheeraj:~$ cat cooltext2.txt
Hello again to new cool test.
masterx@Dheeraj:~$ cp -i cooltext.txt cooltext2.txt
cp: overwrite 'cooltext2.txt'? y
```

## 8.2] `cp -u` 

### This command will  copy only when the SOURCE file is newer than the destination file or when the destination file is missing

```
masterx@Dheeraj:~/timed_text_files$ ls -l
total 8
-rw-r--r-- 1 masterx masterx 50 Feb 24 22:01 newtest.txt
-rw-r--r-- 1 masterx masterx 37 Feb 24 22:00 oldtest.txt
masterx@Dheeraj:~/timed_text_files$ cp -u oldtest.txt newtest.txt
masterx@Dheeraj:~/timed_text_files$ cat newtest.txt
This is new text. This was made after oldtest.txt
masterx@Dheeraj:~/timed_text_files$ cp -u newtest.txt oldtest.txt
masterx@Dheeraj:~/timed_text_files$ cat oldtest.txt
This is new text. This was made after oldtest.txt
masterx@Dheeraj:~/timed_text_files$ ls -l
total 8
-rw-r--r-- 1 masterx masterx 50 Feb 24 22:01 newtest.txt
-rw-r--r-- 1 masterx masterx 50 Feb 24 22:03 oldtest.txt
masterx@Dheeraj:~/timed_text_files$
```


## 8.3] `cp -v`

### This command will explain what is happening
```
masterx@Dheeraj:~/timed_text_files$ ls
newtest.txt  oldtest.txt
masterx@Dheeraj:~/timed_text_files$ cp -v newtest.txt oldtest.txt
'newtest.txt' -> 'oldtest.txt'
masterx@Dheeraj:~/timed_text_files$
```


# 9] `head`

```
masterx@Dheeraj:~/timed_text_files$ head testingLong.txt
The ants enjoyed the barbecue more than the family.
He created a pig burger out of beef.
I love eating toasted cheese and tuna sandwiches.
At that moment he wasn't listening to music, he was living an experience.
The thunderous roar of the jet overhead confirmed her worst fears.
The Japanese yen for commerce is still well-known.
Nobody loves a pig wearing lipstick.
Happiness can be found in the depths of chocolate pudding.
Today arrived with a crash of my car through the garage door.
It was the scarcity that fueled his creativity.
```


```

Usage: head [OPTION]... [FILE]...
Print the first 10 lines of each FILE to standard output.
With more than one FILE, precede each with a header giving the file name.
```

## 9.1] `head -n`

### This command will print the first NUM lines instead of the first 10

```
masterx@Dheeraj:~/timed_text_files$ ls
newtest.txt  oldtest.txt  testingLong.txt
masterx@Dheeraj:~/timed_text_files$ head -3 testingLong.txt
The ants enjoyed the barbecue more than the family.
He created a pig burger out of beef.
I love eating toasted cheese and tuna sandwiches.
masterx@Dheeraj:~/timed_text_files$
```

## 9.2] `head -q`

### This command will never print headers giving file names

```
masterx@Dheeraj:~/timed_text_files$ head -q testingLong.txt
The ants enjoyed the barbecue more than the family.
He created a pig burger out of beef.
I love eating toasted cheese and tuna sandwiches.
At that moment he wasn't listening to music, he was living an experience.
The thunderous roar of the jet overhead confirmed her worst fears.
The Japanese yen for commerce is still well-known.
Nobody loves a pig wearing lipstick.
Happiness can be found in the depths of chocolate pudding.
Today arrived with a crash of my car through the garage door.
It was the scarcity that fueled his creativity.
```


## 9.3] `head -v`

### This command will always print headers giving file names

```
masterx@Dheeraj:~/timed_text_files$ head -v testingLong.txt
==> testingLong.txt <==
The ants enjoyed the barbecue more than the family.
He created a pig burger out of beef.
I love eating toasted cheese and tuna sandwiches.
At that moment he wasn't listening to music, he was living an experience.
The thunderous roar of the jet overhead confirmed her worst fears.
The Japanese yen for commerce is still well-known.
Nobody loves a pig wearing lipstick.
Happiness can be found in the depths of chocolate pudding.
Today arrived with a crash of my car through the garage door.
It was the scarcity that fueled his creativity.
```

<br>
<hr>
<br>

# 10] `tail`

```
masterx@Dheeraj:~/timed_text_files$ tail testingLong.txt
She traveled because it cost the same as therapy and was a lot more enjoyable.
The virus had powers none of us knew existed.
Thirty years later, she still thought it was okay to put the toilet paper roll under rather than over.
They looked up at the sky and saw a million stars.
He uses onomatopoeia as a weapon of mental destruction.
The efficiency we have at removing trash has made creating trash more acceptable.
Every manager should be able to recite at least ten nursery rhymes backward.
All you need to do is pick up the pen and begin.
We should play with legos at camp.
Dolores wouldn't have eaten the meal if she had known what it actually was.
masterx@Dheeraj:~/timed_text_files$
```

```
Usage: tail [OPTION]... [FILE]...
Print the last 10 lines of each FILE to standard output.
With more than one FILE, precede each with a header giving the file name.

With no FILE, or when FILE is -, read standard input.
```

## 10.1] `tail -n`

### This command will output the last NUM lines, instead of the last 10

```
masterx@Dheeraj:~/timed_text_files$ tail -3 testingLong.txt
All you need to do is pick up the pen and begin.
We should play with legos at camp.
Dolores wouldn't have eaten the meal if she had known what it actually was.
masterx@Dheeraj:~/timed_text_files$
```

## 10.2] `tail -q`

### This command will never output headers giving file names

```
masterx@Dheeraj:~/timed_text_files$ tail -q testingLong.txt
She traveled because it cost the same as therapy and was a lot more enjoyable.
The virus had powers none of us knew existed.
Thirty years later, she still thought it was okay to put the toilet paper roll under rather than over.
They looked up at the sky and saw a million stars.
He uses onomatopoeia as a weapon of mental destruction.
The efficiency we have at removing trash has made creating trash more acceptable.
Every manager should be able to recite at least ten nursery rhymes backward.
All you need to do is pick up the pen and begin.
We should play with legos at camp.
Dolores wouldn't have eaten the meal if she had known what it actually was.
masterx@Dheeraj:~/timed_text_files$
```
 
## 10.3] `tail -v` 

### This command will always output headers giving file names

```
masterx@Dheeraj:~/timed_text_files$ tail -v testingLong.txt
==> testingLong.txt <==
She traveled because it cost the same as therapy and was a lot more enjoyable.
The virus had powers none of us knew existed.
Thirty years later, she still thought it was okay to put the toilet paper roll under rather than over.
They looked up at the sky and saw a million stars.
He uses onomatopoeia as a weapon of mental destruction.
The efficiency we have at removing trash has made creating trash more acceptable.
Every manager should be able to recite at least ten nursery rhymes backward.
All you need to do is pick up the pen and begin.
We should play with legos at camp.
Dolores wouldn't have eaten the meal if she had known what it actually was.
masterx@Dheeraj:~/timed_text_files$
```


<br>
<hr>
<br>



# 11] `sort`

```
masterx@Dheeraj:~/timed_text_files$ cat randomWords.txt
Zebra
Cat
Ball
Apple
Enter
Mask
Horse
masterx@Dheeraj:~/timed_text_files$ sort randomWords.txt
Apple
Ball
Cat
Enter
Horse
Mask
Zebra
masterx@Dheeraj:~/timed_text_files$
```

```
Usage: sort [OPTION]... [FILE]...
  or:  sort [OPTION]... --files0-from=F
Write sorted concatenation of all FILE(s) to standard output.
```

## 11.1] `sort -r filename`

### This command will sort all files in reverse

```
masterx@Dheeraj:~/timed_text_files$ sort -r numbers.txt
1000000000
10000000
100000
10000
1000
100
10
1
```

## 11.2] `sort filename -o outputFilename`

### This command will store the output of the file in the specified file

```
masterx@Dheeraj:~/timed_text_files$ sort numbers.txt -o output.txt
masterx@Dheeraj:~/timed_text_files$ ls
newtest.txt  oldtest.txt  randomWords.txt
numbers.txt  output.txt   testingLong.txt
masterx@Dheeraj:~/timed_text_files$ cat output.txt
1
10
100
1000
10000
100000
10000000
1000000000
masterx@Dheeraj:~/timed_text_files$
```


## 11.3] `sort -V filename`

### This command  natural sort of (version) numbers within text

```
masterx@Dheeraj:~/timed_text_files$ sort testingLong.txt -V
After exploring the abandoned building, he started to believe in ghosts.
All you need to do is pick up the pen and begin.
At that moment he wasn't listening to music, he was living an experience.
Dolores wouldn't have eaten the meal if she had known what it actually was.
Every manager should be able to recite at least ten nursery rhymes backward.
Happiness can be found in the depths of chocolate pudding.
He created a pig burger out of beef.
He uses onomatopoeia as a weapon of mental destruction.
In that instant, everything changed.
It took him a month to finish the meal.
It was a slippery slope and he was willing to slide all the way to the deepest depths.
It was the scarcity that fueled his creativity.
```

<br>
<hr>
<br>


# 12] `wc`


```
masterx@Dheeraj:~/timed_text_files$ wc testingLong.txt
  29  339 1856 testingLong.txt
```



```
Usage: wc [OPTION]... [FILE]...
  or:  wc [OPTION]... --files0-from=F
Print newline, word, and byte counts for each FILE, and a total line if
more than one FILE is specified.  A word is a non-zero-length sequence of
characters delimited by white space.
```

## 12.1] `wc -c filename`

### This command will print the byte counts

```
masterx@Dheeraj:~/timed_text_files$ wc -c testingLong.txt
1856 testingLong.txt
```


## 12.2] `wc -m filename`

### This command will print the character counts

```
masterx@Dheeraj:~/timed_text_files$ wc -m testingLong.txt
1854 testingLong.txt
```



## 12.3] `wc -w filename`
### This command will print the word count

```
masterx@Dheeraj:~/timed_text_files$ wc -w testingLong.txt
339 testingLong.txt
```


<br>
<hr>
<br>


# 13] `chown`


```
Usage: chown [OPTION]... [OWNER][:[GROUP]] FILE...
  or:  chown [OPTION]... --reference=RFILE FILE...
This commandd will change the owner and/or group of each FILE to OWNER and/or GROUP.
With --reference, change the owner and group of each FILE to those of RFILE.
```

## 13.1] `chown -f`

### This command will suppress most error messages

## 13.2] `chown -h`

### This command affect symbolic links instead of any referenced file useful only on systems that can change the ownership of a symlink 

## 13.3] `chown -R`

### This command will operate on files and directories recursively

<br>
<hr>
<br>




# 14] `chmod`

```
masterx@Dheeraj:~/timed_text_files$ ls -l
total 32
-rw-r--r-- 1 masterx masterx   57 Feb 24 22:45 namedNumbers.txt
-rw-r--r-- 1 masterx masterx   50 Feb 24 22:01 newtest.txt
-rw-r--r-- 1 masterx masterx   47 Feb 24 22:37 numbers.txt
-rw-r--r-- 1 masterx masterx   50 Feb 24 22:04 oldtest.txt
-rw-r--r-- 1 masterx masterx   47 Feb 24 22:41 output.txt
-rw-r--r-- 1 masterx masterx   68 Feb 24 22:48 randomThings2.txt
-rw-r--r-- 1 masterx masterx   38 Feb 24 22:33 randomWords.txt
-rw-r--r-- 1 masterx masterx 1856 Feb 24 22:10 testingLong.txt
masterx@Dheeraj:~/timed_text_files$ chmod 777 testingLong.txt
masterx@Dheeraj:~/timed_text_files$ ls -l
total 32
-rw-r--r-- 1 masterx masterx   57 Feb 24 22:45 namedNumbers.txt
-rw-r--r-- 1 masterx masterx   50 Feb 24 22:01 newtest.txt
-rw-r--r-- 1 masterx masterx   47 Feb 24 22:37 numbers.txt
-rw-r--r-- 1 masterx masterx   50 Feb 24 22:04 oldtest.txt
-rw-r--r-- 1 masterx masterx   47 Feb 24 22:41 output.txt
-rw-r--r-- 1 masterx masterx   68 Feb 24 22:48 randomThings2.txt
-rw-r--r-- 1 masterx masterx   38 Feb 24 22:33 randomWords.txt
-rwxrwxrwx 1 masterx masterx 1856 Feb 24 22:10 testingLong.txt
masterx@Dheeraj:~/timed_text_files$
```


```
Usage: chmod [OPTION]... MODE[,MODE]... FILE...
  or:  chmod [OPTION]... OCTAL-MODE FILE...
  or:  chmod [OPTION]... --reference=RFILE FILE...
This command changes the mode of each FILE to MODE.
```

## 14.1] `chmod -c MODE FILE`

### This command writes a message if a mode is changed

```
masterx@Dheeraj:~/timed_text_files$ ls -l
total 32
-rw-r--r-- 1 masterx masterx   57 Feb 24 22:45 namedNumbers.txt
-rw-r--r-- 1 masterx masterx   50 Feb 24 22:01 newtest.txt
-rw-r--r-- 1 masterx masterx   47 Feb 24 22:37 numbers.txt
-rw-r--r-- 1 masterx masterx   50 Feb 24 22:04 oldtest.txt
-rw-r--r-- 1 masterx masterx   47 Feb 24 22:41 output.txt
-rw-r--r-- 1 masterx masterx   68 Feb 24 22:48 randomThings2.txt
-rw-r--r-- 1 masterx masterx   38 Feb 24 22:33 randomWords.txt
-rwxrwxrwx 1 masterx masterx 1856 Feb 24 22:10 testingLong.txt
masterx@Dheeraj:~/timed_text_files$ chmod -c 666 testingLong.txt
mode of 'testingLong.txt' changed from 0777 (rwxrwxrwx) to 0666 (rw-rw-rw-)
masterx@Dheeraj:~/timed_text_files$
```


## 14.2] `chmod -v MODE FILE(s)`
### This command outputs a diagnostic for every file processed

```
masterx@Dheeraj:~/timed_text_files$ ls -l
total 32
-rw-r--r-- 1 masterx masterx   57 Feb 24 22:45 namedNumbers.txt
-rw-r--r-- 1 masterx masterx   50 Feb 24 22:01 newtest.txt
-rw-r--r-- 1 masterx masterx   47 Feb 24 22:37 numbers.txt
-rw-r--r-- 1 masterx masterx   50 Feb 24 22:04 oldtest.txt
-rw-r--r-- 1 masterx masterx   47 Feb 24 22:41 output.txt
-rw-r--r-- 1 masterx masterx   68 Feb 24 22:48 randomThings2.txt
-rw-r--r-- 1 masterx masterx   38 Feb 24 22:33 randomWords.txt
-rw-rw-rw- 1 masterx masterx 1856 Feb 24 22:10 testingLong.txt
masterx@Dheeraj:~/timed_text_files$ chmod -v 666 output.txt numbers.txt namedNumbers.txt testingLong.txt
mode of 'output.txt' changed from 0644 (rw-r--r--) to 0666 (rw-rw-rw-)
mode of 'numbers.txt' changed from 0644 (rw-r--r--) to 0666 (rw-rw-rw-)
mode of 'namedNumbers.txt' changed from 0644 (rw-r--r--) to 0666 (rw-rw-rw-)
mode of 'testingLong.txt' retained as 0666 (rw-rw-rw-)
```

## 14.3] `chmod -R`
### This command will change files and directories recursively

```
masterx@Dheeraj:~$ ls -l
total 28
drwxr-xr-x 3 masterx masterx 4096 Feb 24 20:34 boringAssingments
-rw-r--r-- 1 masterx masterx   50 Feb 24 21:58 cooltext2.txt
-rw-r--r-- 1 masterx masterx   50 Feb 24 21:57 cooltext.txt
-rwxrwxrwx 1 masterx masterx   20 Feb 18 13:09 data.txt
drwxr-xr-x 3 masterx masterx 4096 Feb 24 23:23 ftrax
drwxr-xr-x 2 masterx masterx 4096 Feb 24 22:47 timed_text_files
drwxr-xr-x 2 masterx masterx 4096 Feb 24 21:47 videos
masterx@Dheeraj:~$ chmod -f -R 104 ftrax/*
masterx@Dheeraj:~$ ls -l
total 28
drwxr-xr-x 3 masterx masterx 4096 Feb 24 20:34 boringAssingments
-rw-r--r-- 1 masterx masterx   50 Feb 24 21:58 cooltext2.txt
-rw-r--r-- 1 masterx masterx   50 Feb 24 21:57 cooltext.txt
-rwxrwxrwx 1 masterx masterx   20 Feb 18 13:09 data.txt
drwxr-xr-x 3 masterx masterx 4096 Feb 24 23:23 ftrax
drwxr-xr-x 2 masterx masterx 4096 Feb 24 22:47 timed_text_files
drwxr-xr-x 2 masterx masterx 4096 Feb 24 21:47 videos
```


<br>
<hr>
<br>

# 15]  `chgrp`

```
Usage: chgrp [OPTION]... GROUP FILE...
  or:  chgrp [OPTION]... --reference=RFILE FILE...
Change the group of each FILE to GROUP.
With --reference, change the group of each FILE to that of RFILE.
```


## 15.1] `chgrp -c`

### This command is like verbose but report only when a change is made


## 15.2] `chgrp -v`

### This command output a diagnostic for every file processed

## 15.3] `chgrp -f`

### This command suppress most error messages


<br>
<hr>
<br>

# 16] `umask`

```
masterx@Dheeraj:~$ umask
0022
masterx@Dheeraj:~$
```

```
umask: umask [-p] [-S] [mode]
    Display or set file mode mask.

    Sets the user file-creation mask to MODE.  If MODE is omitted, prints
    the current value of the mask.

    If MODE begins with a digit, it is interpreted as an octal number;
    otherwise it is a symbolic mode string like that accepted by chmod(1).
```
## 16.1]  `umask -S`

### This command makes the output of umask symbolic instead of OCTAL

```
masterx@Dheeraj:~$ umask -S
u=rwx,g=rx,o=rx
```

## 16.2] `umask -p`

### This command gives the output of umask in OCTAL format

```
masterx@Dheeraj:~$ umask -p
umask 0044
```

<br>
<hr>
<br>

## 17] `ps`

### This command shows the current processes running

```
masterx@Dheeraj:~$ ps
  PID TTY          TIME CMD
    9 pts/0    00:00:00 bash
   55 pts/0    00:00:00 ps
masterx@Dheeraj:~$
```

### 17.1] `ps -v`

```
masterx@Dheeraj:~$ ps -v
  PID TTY      STAT   TIME  MAJFL   TRS   DRS   RSS %MEM COMMAND
    9 pts/0    Ss     0:00     29   885  9166  5016  0.1 -bash
   84 pts/0    R+     0:00      0    86 10433  3164  0.0 ps -v
masterx@Dheeraj:~$
```

<br>
<hr>
<br>

# 18] `" | "`

### The pipe ' | ' helps us execute 2 commands at the same time

```
masterx@Dheeraj:~$ ls -l | head -5
total 60
drwxr-xr-x 2 masterx masterx 4096 Feb 14 21:38 folder1
drwxr-xr-x 2 masterx masterx 4096 Feb 14 21:38 folder10
drwxr-xr-x 2 masterx masterx 4096 Feb 14 21:38 folder11
drwxr-xr-x 2 masterx masterx 4096 Feb 14 21:38 folder12
masterx@Dheeraj:~$
```


```
masterx@Dheeraj:~$ ls -l | sort -V
drwxr-xr-x 2 masterx masterx 4096 Feb 14 21:38 folder1
drwxr-xr-x 2 masterx masterx 4096 Feb 14 21:38 folder2
drwxr-xr-x 2 masterx masterx 4096 Feb 14 21:38 folder3
drwxr-xr-x 2 masterx masterx 4096 Feb 14 21:38 folder4
drwxr-xr-x 2 masterx masterx 4096 Feb 14 21:38 folder5
drwxr-xr-x 2 masterx masterx 4096 Feb 14 21:38 folder6
drwxr-xr-x 2 masterx masterx 4096 Feb 14 21:38 folder7
drwxr-xr-x 2 masterx masterx 4096 Feb 14 21:38 folder8
drwxr-xr-x 2 masterx masterx 4096 Feb 14 21:38 folder9
drwxr-xr-x 2 masterx masterx 4096 Feb 14 21:38 folder10
drwxr-xr-x 2 masterx masterx 4096 Feb 14 21:38 folder11
drwxr-xr-x 2 masterx masterx 4096 Feb 14 21:38 folder12
drwxr-xr-x 2 masterx masterx 4096 Feb 14 21:38 folder13
drwxr-xr-x 2 masterx masterx 4096 Feb 14 21:38 folder14
drwxr-xr-x 2 masterx masterx 4096 Feb 14 21:38 folder15
total 60
masterx@Dheeraj:~$
```


<br>
<hr>
<br>

# 19] `< (output)` & `> (input)`

## These help us in providing the output of one command as input to another

```
masterx@Dheeraj:~/timed_text_files$ ls -l > list_of_files_in_this_directory.txt
masterx@Dheeraj:~/timed_text_files$ ls
list_of_files_in_this_directory.txt  newtest.txt  oldtest.txt  randomThings2.txt  testingLong.txt
namedNumbers.txt                     numbers.txt  output.txt   randomWords.txt
masterx@Dheeraj:~/timed_text_files$ cat list_of_files_in_this_directory.txt
total 32
-rw--w--w- 1 masterx masterx    0 Feb 25 04:04 list_of_files_in_this_directory.txt
-rw-rw-rw- 1 masterx masterx   57 Feb 24 22:45 namedNumbers.txt
-rw-r--r-- 1 masterx masterx   50 Feb 24 22:01 newtest.txt
-rw-rw-rw- 1 masterx masterx   47 Feb 24 22:37 numbers.txt
-rw-r--r-- 1 masterx masterx   50 Feb 24 22:04 oldtest.txt
-rw-rw-rw- 1 masterx masterx   47 Feb 24 22:41 output.txt
-rw-r--r-- 1 masterx masterx   68 Feb 24 22:48 randomThings2.txt
-rw-r--r-- 1 masterx masterx   38 Feb 24 22:33 randomWords.txt
-rw-rw-rw- 1 masterx masterx 1856 Feb 24 22:10 testingLong.txt
masterx@Dheeraj:~/timed_text_files$
```


```
masterx@Dheeraj:~/timed_text_files$ sort < namedNumbers.txt
One1
One10
One100
One1000
One10000
One100000
One10000000
masterx@Dheeraj:~/timed_text_files$
```

# Q. 20 

# A] Display top 10 processes in descending order

## `ps -eo pid,ppid,cmd,%mem,%cpu --sort=-%mem | head -10`

```
masterx@Dheeraj:~/ftrax/nextFolder$ ps -eo pid,ppid,cmd,%mem,%cpu --sort=-%mem | head -10
  PID  PPID CMD                         %MEM %CPU
    9     8 -bash                        0.0  0.0
   79     9 ps -eo pid,ppid,cmd,%mem,%c  0.0 10.0
    1     0 /init                        0.0  0.0
   80     9 head -10                     0.0  1.0
    8     7 /init                        0.0  0.0
    7     1 /init                        0.0  0.0
masterx@Dheeraj:~/ftrax/nextFolder$
```

<br>
<hr>
<br>

# B] Display the process with highest memory usage.

## `ps -aux --sort -pid`

```
masterx@Dheeraj:~$ ps -aux --sort -pid
USER       PID %CPU %MEM    VSZ   RSS TTY      STAT START   TIME COMMAND
masterx     40 24.0  0.0  10628  3068 pts/0    R+   01:50   0:00 ps -aux --sort -pid
masterx      9  0.0  0.0   7100  3880 pts/0    Ss   00:51   0:01 -bash
root         8  0.0  0.0   1732    84 ?        S    00:51   0:00 /init
root         7  0.0  0.0   1732    68 ?        Ss   00:51   0:00 /init
root         1  0.0  0.0   1712  1052 ?        Sl   00:51   0:00 /init
```


# C] Display current user logged in and logname.

## `whoami`

## `logname`

```
masterx@Dheeraj:~/ftrax/nextFolder$ whoami
masterx
masterx@Dheeraj:~/ftrax/nextFolder$ logname
logname: no login name
masterx@Dheeraj:~/ftrax/nextFolder$
```


# D] Display current shell, home directory, operating system type, current path setting, current working directory.


## `echo "$SHELL"`

```
masterx@Dheeraj:~/ftrax/nextFolder$ echo "$SHELL"
/bin/bash
masterx@Dheeraj:~/ftrax/nextFolder$
```

## `echo "$HOME"`

```
masterx@Dheeraj:~/ftrax/nextFolder$ echo "$HOME"
/home/masterx
masterx@Dheeraj:~/ftrax/nextFolder$
```

## `echo $PATH`

```
masterx@Dheeraj:~/ftrax/nextFolder$ echo "$PATH"
/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/games:/usr/local/games:/mnt/c/oraclexe/app/oracle/product/11.2.0/server/bin:/mnt/c/Users/USER/AppData/Local/Programs/Python/Python39/Scripts/:/mnt/c/Users/USER/AppData/Local/Programs/Python/Python39/:/mnt/c/Python37/Scripts/:/mnt/c/Python37/:/mnt/c/WINDOWS/system32:/mnt/c/WINDOWS:/mnt/c/WINDOWS/System32/Wbem:/mnt/c/WINDOWS/System32/WindowsPowerShell/v1.0/:/mnt/c/Program Files/dotnet/:/mnt/c/Program Files/Intel/WiFi/bin/:/mnt/c/Program Files/Common Files/Intel/WirelessCommon/
```



## `pwd`

```
masterx@Dheeraj:~/ftrax/nextFolder$ pwd
/home/masterx/ftrax/nextFolder
masterx@Dheeraj:~/ftrax/nextFolder$
```


# E] Display current

## `cat /etc/os-release` 

```
masterx@Dheeraj:~/ftrax/nextFolder$ cat /etc/os-release
PRETTY_NAME="Debian GNU/Linux 10 (buster)"
NAME="Debian GNU/Linux"
VERSION_ID="10"
VERSION="10 (buster)"
VERSION_CODENAME=buster
ID=debian
HOME_URL="https://www.debian.org/"
SUPPORT_URL="https://www.debian.org/support"
BUG_REPORT_URL="https://bugs.debian.org/"
masterx@Dheeraj:~/ftrax/nextFolder$
```

## `uname -a`

```
masterx@Dheeraj:~$ uname -a
Linux Dheeraj 5.4.72-microsoft-standard-WSL2 #1 SMP Wed Oct 28 23:40:43 UTC 2020 x86_64 GNU/Linux
masterx@Dheeraj:~$
```