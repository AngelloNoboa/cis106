---
Name: Angello Noboa
Semester: fall 22
Course: CIS-106 Linux Fund
---

# Question 1

## awk
* Description:
* Formula:
* Examples:

## cat
* Description: cat(Concatenate)is used for displaying the content of a file.
* Formula: `cat + option + file(s) to display`
* Examples:
  * Display the content of a file using absolute path
    * `cat ~/Documents/todo.lst`
  * Display the content of a file with line numbers
    * `cat -n ~/Documents/todo.md`
  * Display the content of a file a $ at the end of every line
    * `cat -E ~/Documents/todo.md`

## cp
* Description: copies files/directories from a source to a destination
* Formula:
  * For any destination use
    * `cp + files to copy + destination`
  * for copying directories use
    * `cp -r + directory to copy + destination`
* Examples:
  * TO copy a file
    * `cp Downloads/wallpapers.zip  Pictures/`
  * To copy the content of a directory to another directory using willcard
    * `cp Downloads/wallpapers/*  ~/Pictures/`
  * To copy multiple files in a single command
    * `sudo cp -r script.sh program.py home.html assets/  /var/www/html/`

## cut
* Description: Cut is used to extract a specific section of each line of a file and display it to the screen.
* Formula: `cut + option + file(s)`
* Examples:
  * Display a list of all the users in your system
    * `cut -d ':' -f1 /ect/passwd`
  * Display a list of all the users in your system with their login shell
    * `cut -d ':' -f1,7 /ect/passwd`
  * Cut a file using a delimiter but changing the delimiter in the output.
    * `cut -d ',' -f1,7 --output-delimiter= '=>' /ect/passwd`
  * Cut a file excluding a given field
    * `cut -d ',' --complement -s -f3 users.txt` 

## grep
* Description: Grep is used to search text in given file
* Formula: `grep + option + search criteria + file(s)`
* Examples:
  * Search any line that contains the word "dracula" in the given file
    * `grep 'dracula' ~/Documents/dracula.txt`
  * Search any line that contains the word dracula regardless of case and with number line
    * `grep -in 'dracula ~/Documents/Books/dracula.txt'`
  * Search for all the lines that do not contain the word 'war'
    * `grep -v 'war' ~/Documents/Books/war-and-peace.txt`
  * Search and display only the matched string(pattern)
    * `grep -o 'pride' ~/Documents/Books/war-and-peace.txt`
  * Display every line that starts with an upper case letter or a number in the book dracula.
    * `grep -E "^[A-Z][0-9]" dracula.txt`

## head
* Description: Head displays the top N numbers of lines of a given file.
* Formula: `head + option + file(s)` 
* Examples:
  * Display the first 10 lines of a file
    * `head ~/Documents/Book/dracula.txt`
  * Display the first 5 lines of a file
    * `head -5 ~/Documents/Book/dracula.txt`

## ls
* Description: used for listing the content of a giving directory or the file/directory itself.
* Formula: `ls + option + directory to list`
* Examples:
  * List all the files inside a given directory (also hidden files)
    * `ls -a ~/Pictures`
  * Long list all the files inside a given directory recursively and with human readable size
    * `ls -lRh ~/Pictures`
  * List all files that do not have a vowel after letter f
    * `ls f[!aeiou]*`
  * 

## man
* Description: man(manual) are document files that describe Linux shell command, executable programs, system calls, special files, and so forth. to exit man page press letter "q"
* Formula: `man ls` 
* Examples:
  * Open the man page of the ls command
    * `man ls`
  * Open the man page of the ls command with a specific word been search for
    * `man ls | grep "group"`

## mkdir
* Description: is used for creating a single directory or multiple directories
* Formula: `mkdir + the name of the directory`
* Examples:
  * Create a directory with a single quote in the name
    * `mkdir wallpapers/"majora's mask" `
  * Create multiple directories
    * `mkdir wallpaper/cars wallpapers/cities wallpapers/forest`
  * Create a directory with a ***parent directory*** at the same time
    * `mkdir -p wallpaper_other/movies`

## mv
* Description: moves and renames directories
* Formula: 
  * The basic formula of the mv command is:
    * `mv + source + destination`
  * For renaming files/directories the formula remains the same
    * `mv + file/directory to rename + new name`
* Examples:
  * **Moving File**
    * To move a directory from on directory to another using absolute path
      * `sudo mv ~/Downloads/theme  /urs/share/themes`
    * To move a file from one directory to another combining absolute path and relative path
      * `mv Downloads/english_homework.docx  /media/student/flashdrive` 
    * To move multiple directories/files to a different directory
      * `mv games/ wallpapers/ rockmusic/  /media/student/flashdrive/`
  * **Renaming a file**
    * To rename a file
      * `mv homework.docx cis106homework.docx`
    * To rename a file using absolute path
      * `mv ~/Downloads/homework.docx  ~/Downloads/cis106homework.docx`
    * To move and rename a file in the same command
      * `mv Downloads/cis106homework.docx  Documents/new_cis106homework.docx`

## tac
* Description: Tac(concatenates) is used for displaying the content of a file in reverse order.
* Formula: `tac + option + file(s) to display`
* Examples:
  * Display the content of a file located in the pwd
    * `tac todo.md`
  * Display the content of a file using absolute path
    * `tac ~/Documents/todo.md`

## tail
* Description: Tail displays the last N number of lines of a given file.
* Formula: `tail + option + file`
* Examples:
  * Display the last 10 lines of a file
    * `tail ~/Documents/Book/dracula.txt`
  * Display the last 5 lines of a file
    * `tail -5 ~/Documents/Book/dracula.txt`

## touch
* Description: Is used for creating files
* Formula: `touch + name of file`
* Examples:
  * To create several files
    * `touch list_of_cars.txt script.py names.csv`
  * To create a file with a space in its name:
    * `touch "list of foods.txt"`
  * To create multiple files in different directories with brace expansion
    * `touch  /games/{video_game1.py, video_game2}/documents/{file1.doc, file2.doc}`

## tr
* Description: Tr used to replace a character 
* Formula: `tr + 'original character' 'change character'`
* Examples:
  * Replace the ; for a , in the cereal.csv file
    * `cat cereal.csv | tr ';' ','`

## tree
* Description: Tree will display the whole files/directories in a specific structure
* Formula: `tree + directory `
* Examples:
  * Show all the directories and files in the directory Documents
    * `tree Documents/`

## vim/nano
* Description:
* Formula:
* Examples:


# Question 2

## How to work with multiple terminals open?
* In order to work with multiple terminals we could open two terminals or open Tilix which we can use one terminal for coding while the other could be use for any guidance.

## How to work with manual pages?
* to work with the manual pages use `man + shell command` this will show a list of all the description that could be done with the shell command

## How to parse (search) for specific words in the manual page
* if you need to search a specific word use `man + shell command | grep "specific word"` which will show the result use for with the word been search for

## How to redirect output (> and |)


## How to append the output of a command to a file


## How to use wildcards
* **Wilcard represent letters and characters used to specify a file name for searches**
* `shell command + file name`
### Examples:
  * **Using (*)** 
  * List all the files that ends in .txt
    * `ls *.txt`
  * List all the files that have any letter before the string "file." and after as well
    * `ls *file.*`

  * For copying and moving multiple files at the same time
    * `mv`

## How to use brace expansion
* **Brace expansion {} is not a wilcard but another feature of bash that allows you to generate arbitrary to use with command.**
  *  For creating entire directory structures in a single command
     *  `mkdir -p music/{jazz,rock}/{mp3files,vidoes, oggfile}/new{1..3}`