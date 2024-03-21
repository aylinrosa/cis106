# Notes 2: The Linux FS

Commands cover in lecture:

## File System
### Definition :
The way files are stored and organized.
### Usage 
`ls` + `option` + `directory to list`
### Examples:
* List all files and directories including hidden ones
   * `ls -a`
 * Display detailed information about files and directories
   * `ls -1`
* Display contents of specified directory
   * `ls /path/to/directory`
 <hr>

## Pathname
### Definition :
Location of the file in the files system (Like an address).
### Usage
`cd` + `ls` + `cp`
### Examples:
* Change current directory to documents 
  * `cd Documents`
* List all files and directories indcluding hidden ones
  * `ls -la`
* Copy file to another location
   * `cp file1.txt /path/to/destination/`
<hr>

## Absolute path
### Definition :
The location of a file starting at the root of the file system. 
### Usage
`\Users\user\Documents\example.txt`
### Examples:
* Display location starting at root
 * `/home/john/downloads/song/.mp3`
 * `/home/rosa/pictures/cats/.png`
<hr>

## Relative path
### Definition :
The location of a file starting from the current working directory or a directory that is located inside the current working directory. 
### Usage
`Documents/example.txt`
### Examples:
* `Downloads/song.mp3` 
* `Pictures/wallpapers.png`
* `Documents/research.txt`
  <hr>

## Difference between YOUR HOME diectory and THE HOME directory
### Definition:
YOUR HOME directory is where all your files are located. The HOME directory is the parent directory of all the home directories.
### Usage 
* YOUR HOME
   * `~(username)`
 * THE HOME
   * `$HOME`
### Examples
* YOUR HOME directory:
  * `home/maria53` `home/aylinrosa`
* THE HOME directory
   * `home/` 
<hr>

## Child directory
A better name for this is a subdirectory or subfolder. This is a directory inside another directory. 
### Usage
`mkdir`
### Examples:
* Create directory named work inside project directory
  * `mkdir ~/projects/work`
* Create directory named projects in home directory
   * `mkdir ~/projects`
<hr>

## Bash special characters 
Special characters are function like commands that tell the shell to perform a specific action without having to type the complete command. These special characters make working on the command line more efficiently.
### Usage
`*.text` + `|` + `~`
### Examples:
* List all files that contain .text
   * `ls *.txt`
 * Copy all .text files to another directory
   * `cp *.txt /path/to/destination/`
 * Remove all .txt files
  * `rm *.txt`
  <hr>

## Environment variables  
Environment variables store values of a user’s environment and can be used in commands in the shell. These values can be unique to the user’s environment which makes them ideal when writhing commands that you want to use regales of which user is using the computer.
### Usage 
`$USER` + `$HOME` + `$PWD`
### Examples:
 * Print username of current user
   * `echo $USER`
 * Print absolute path to user's home directory 
   * `echo $HOME`
 * Print absolute path to current working directory
   * `home/user/Documents`
<hr>

## User defined variables 
stores the current’s user username
### Usage
`$USER` 
### Examples
* Create directory with Username
   * `mkdir /tmp/$USER_directory`
 * Copy files to user's home directory
   * `cp file.txt /home/$USER/`
 * Check all files under user's home directory
   * `ls -1 /home/$USER/`
  <hr>

## Usage of $ with variables in bash shell script
Used to access the value stored in a variable
### Usage
 `#!/bin/bash` + `echo $`
### Examples
* Display Users name
   * ` echo -e "\tNAME: \t$name"`
 * Display users age
   * `echo -e "\tAge: \t$age"` 
 * Display users email
   * `echo -e " "\tEmail: \t$email"`
