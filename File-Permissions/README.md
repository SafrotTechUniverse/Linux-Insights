<img alt="File-Permissions" src="../assets/File-Permissions.png" />

### What are the file permissions in Linux?

- In Linux and other Unix-like operating systems, file permissions are a set of rules that determine how a file or directory can be accessed or modified.
- File permissions are represented by a three-part code, typically displayed as a string of characters, such as "rwxr-xr--".
- Each part of the code corresponds to a specific permission group: owner, group, and others.
- The ```ls``` command, coupled with the ```-l``` option (for long listing), provides metadata about your Linux files, revealing details such as the permissions configured for each file.

```
aziz@pop-os:~/my-Files$ ls -l
total 4
drwxrwxr-x 2 aziz aziz 4096 Dec 11 07:56 DirOne
-rw-rw-r-- 1 aziz aziz    0 Dec 11 07:55 main.sh

```
- Permission Attributes


| Permission | For Files | For Directories |
| :---         |     :---:      |          :---:                                                                                                 |
|  Read (r)    | Alows reading the contents of the file.                 | Allows listing the contents of the directory.                        |
| Write (w)    | Allows modifying the contents of the file.             | Allows creating, deleting, or renaming files within the directory.    |
| Execute (x)  | Allows executing the file if it is a program or script | Allows accessing and navigating through the directory. <br> e.g., ```cd directory```           |
