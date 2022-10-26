---
Name: Angello Noboa
Semester: Fall 22
Course: cis-106 Linux Fund
---

# Week Report 5

## What are Command Options?
Command Options are used to modify/enhance their behavior.

## What are Command Arguments?
Command Arguments are the items open which the command acts on.

## Which command is used for creating directories? Provide at least 3 examples.
The command used for creating directories is: `mkdir`

In order to create a directory there is a formula that needs to be follow.
**Formula:** `mkdir + directory name` 

#### Examples:
1. Create a directory in the present working directory
   `mkdir wallpapers`  
2. Create a directory with a space in the name
   `mkdir wallpapers/'cities usa'`
3. Create multiple directories
   `mkdir wallpapers/cars wallpapers/cities wallpaper/forest`
4. Create a directory with a parent directory at the same time.
   `mkdir -p wallpapers_others/movies`

## What does the touch command do? Provide at least 3 examples.
The command touch is used for creating files: `touch`

When creating files using the command touch, follow the formula.
**Formula:** `touch + file name`

#### Examples:
1. Create a file called list
   `touch list`
2. Create file using absolute path
   `touch ~/Downloads/games.txt`
3. Create several files
   `touch list_of_cars.txt script.py names.csv`
4. Create a file with a space in its name
   `touch "list of foods.txt`

## How do you remove a file? Provide an example.
In order to remove a file used the command: `rm`

#### Examples:
1. Remove a file
   `rm list`
2. Remove a file and prompt confirmation before removal
   `rm -i list`
3. Remove all the files inside a directory and ask before removing more than 3 files
   `rm -I Downloads/games/*`


## How do you remove a directory and can you remove non-empty directories in Linux? Provide an example
To remove a directory used the command: `rmdir`
A non-empty directory can be remove by using the command: `rm -r`

#### Examples:
1. Remove an empty directory
   `rmdir Downloads/games`
2. Remove a non-empty directory
   `rm -r Downloads/games`

## Explain the mv and cp command. Provide at least 2 examples of each
***Moving command*** can moves and renames directories by using the command: `mv`

##### There are two different formula to use with the moving command
* The basic formula of the mv command is:
   `mv + source + destination`
* To rename files/directories the formula remains the same: 
   `mv + file/directory to rename + new name`

#### Moving Examples:
1. To remove a file from a directory to another using relative path
   `mv Downloads/homework.pdf Documents/`
2. To move a file one directory to another combining absolute path and relative path
   `mv Downloads/english_homework.docx  /media/student/flashdrive/`
3. To move multiple directories/files to a different directory
   `mv games/ wallpapers/ rockmusic/  /media/student/flashdrive/`

#### Renaming Examples:
1. To rename a file
   `mv homework.docx cis106homework.docx`
2. To rename a file using absolute path
   `mv ~/Downloads/homework.docx  ~/Downloads/cis106homework.docx`
3. To move and rename a file in the same command
   `mv Downloads/cis106homework.docx  Documents/new_cis106homework.docx`


***Copying Command*** can copies file/directories from a source to a destination by using the command: `cp`

When using the command copy always remember to follow the formula.
**Formula:** `cp + files to copy + destination`

#### Examples:
1. copy a file
   `cp Downloads/wallpapers.zip  Pictures/`
2. Copy a directory with absolute path
   `cp -r ~/Downloads/wallpapers  ~/Pictures/`
3. Copy the content of a directory to another directory
   `cp Downloads/wallpapers/*  ~/Pictures/`
4. Copy multiple files in a single command
   `sudo cp -r script.sh program.py home.html  assets/  /var/www/html/` 


## Practice

* Practice 1
[p1](p1.png)<br>
* Practice 2
[p2](p2.png)<br>
* Practice 3
[p3](p3.png)<br>
[p3](p3.2.png)<br>
[p3](p3.3.png)<br>
* Practice 4
[p4](p4.png)