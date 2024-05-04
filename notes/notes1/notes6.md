# Notes 6: Handling files

## Awk
### Definition
is a scripting language used for processing text files. AWK supports almost if not all of the features of a programming language. 
### Usage:
`awk 'pattern { action }' file`
### Example: 
* Print the second column of a CSV file:
`awk -F',' '{print $2}' data.csv`
### Example: 
* Filter lines containing a specific pattern
`awk '/pattern/' file.txt`

## Sed
### Definition:
a stream editor that performs operations on files. Just like AWK, SED can be complex and tough to master however, as a Linux user you must at least be familiar with its basic functionality
### Usage:
`sed 's/old_text/new_text/' file`
### Example:
* Replace "foo" with "bar" in a file:
`sed 's/foo/bar/' file.txt`
* Delete lines containing a specific pattern:
* `sed '/pattern/d' file.txt`


## Less
### Definition
a terminal pager program that allows you to view text files one page at a time. It provides navigation and search functionalities to easily scroll through large files.
### Usage:
`less file`
### Example: 
* View the contents of a file:
`less README.md`
* Search for a specific term within the file:
`less large_file.log
/search_term`

## Alias
### Definition
used to create shortcuts or abbreviations for longer commands. It allows you to define custom command aliases to simplify repetitive tasks or to create personalized shortcuts.
### Usage:
`alias new_command='original_command'`
### Example: 
* Create an alias for listing files with detailed information
`alias ll='ls -l'`
* Create an alias for navigating to a specific directory:
`alias mydir='cd /path/to/my/directory'`


