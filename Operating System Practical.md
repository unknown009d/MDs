# Operating System Practical


#### <u>ls</u> : List Directory Content

```bash
$ ls
newFolder1/ newFolder2/ newFolder3/
```

#### <u>ls -al</u> : a=showAll, l=longListingFormat

```bash
$ ls -al
drwxr-xr-x 47 username username 4096 Feb 7 22:27 ./
drwxr-xr-x 4 root root 4096 Dec 17 20:26 ../
drwxr-xr-x 4 root root 4096 Dec 17 20:26 newFolder1/
drwxr-xr-x 4 root root 4096 Dec 17 20:26 newFolder2/
drwxr-xr-x 4 root root 4096 Dec 17 20:26 newFolder3/
```

#### <u>ls -lt</u> : l=longListingFormat, t=showLatestEditedFileFirst

```bash
$ ls -lt
drwxr-xr-x 47 username username 4096 Feb 7 22:27 ./
drwxr-xr-x 4 root root 4096 Dec 17 20:26 ../
drwxr-xr-x 4 root root 4096 Dec 17 20:26 newFolder1/
drwxr-xr-x 4 root root 4096 Dec 17 20:26 newFolder2/
drwxr-xr-x 4 root root 4096 Dec 17 20:26 newFolder3/
```

#### <u>cd  dir</u> : Change Directory with parameter of the location of the directory

```bash
$ cd newFolder1
newFolder/ $ pwd
/home/user/newFolder
```

#### <u>cd</u> : Change directory to the home folder of the current user

```bash
newFolder/ $ cd
$
```

#### <u>pwd</u> : Output the current working directory

```bash
$ pwd
/home/user
```

#### <u>mkdir dir</u>  : make directories with directory name as parameter

```bash
$ mkdir newFolder4
```

#### <u>cat > filename</u> : concatenate files and print on the standard output

```bash
$ cat > filename.txt
This is a simple text
and this is the second line
^C
$
```

#### <u>more filename</u> : file perusal filter for crt viewing

```bash
$ more filename.txt
This is a simple text
and this is the second line
$
```

#### <u>head file</u> : output the first part of files

```bash
$ head -n filename.txt
This is a simple text
$
```

#### <u>tail file</u> : output the last part of files

```bash
$ tail filename.txt
This is a simple text
and this is the second line
$
```

#### <u>tail -f file</u> : output appended data as the file grows

```bash
$ tail filename.txt
This is a simple text
and this is the second line
^C
$
```

#### **<u>touch file</u>** : Change file timestamps

```bash
$ touch newFolder1/newFile.txt
$ head newFolder1/newFile.txt
$ 
```

#### **<u>rm file</u>** : Remove files or directories

```bash
$ rm filename.txt
$ ls
newFolder1/ newFolder2/ newFolder3/ newFolder4/
$
```

#### <u>rm -r dir</u> : Remove directories and their contents recursively

```bash
$ rm -r newFolder1/newFile.txt
$ ls
newFolder2/ newFolder3/ newFolder4/

```

#### <u>rm -f file</u> : Ignore nonexistent files and arguments, never prompt

```bash
$ rm -f newFolder2
$ ls
newFolder3/ newFolder4/
$
```

#### <u>rm -rf dir</u> : Remove directories recursively

```bash
$ rm -rf newFolder3
$ ls
newFolder4/
$
```

#### <u>cp file1 file2</u> : Copy files and directories

```bash
$ echo "NewFile" > sample.txt
$ ls
newFolder4/ sample.txt
$ cp sample.txt copySample.txt
$ ls
newFolder4/ sample.txt copySample.txt
$
```

#### <u>cp -r dir1 dir2</u> : Copy files or directories recursively

```bash
$ mkdir newFolder
$ echo "haha" > newFolder/new.txt
$ cp newFolder/new.txt newFolder4/
$ ls
newFolder/ newFolder4/ sample.txt copySample.txt
$
```

#### <u>mv file1 file2</u> : Move (rename) files

```bash
$ mv sample.txt newFolder
$ ls
newFolder/ newFolder4/ copySample.txt
$ ls newFolder/
new.txt sample.txt
$
```

#### <u>**ln -s file link**</u> : Make -s=symbolic links between files

```bash
$ ln -s newFolder/sample.txt linkedOld
$ ls
linkOld@ newFolder/ newFolder4/ copySample.txt
```





