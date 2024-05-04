# Notes 3: Managing Files and Directories

Commands covered in lecture

## Mkdir 
### Definition:
used for creating a single directory or multiple directories. 
### Usage
`mkdir + directory_name`
### Example
Create a directory named "docs":
* `mkdir docs`
 Create multiple directories named "images", "videos", and "music":
 *  `mkdir images videos music`
Create a directory with spaces in the name:
* `mkdir "mkdir "my documents"`


## Touch 
### Definition: 
4Creates empty files or updates the access and modification timestamps of existing files.
### Usage: 
`touch file_name`
### Example:
* Create an empty file named "notes.txt":
`touch notes.txt`
* Update the timestamp of an existing file named "report.doc":
`touch report.doc`

## Rm
### Definition: 
Removes files or directories.
### Usage: 
`rm file_name`
### Example:
* Remove a file named "oldfile.txt":
`rm oldfile.txt`
* Remove multiple files named "file1.txt", "file2.txt", and "file3.txt":
`rm file1.txt file2.txt file3.txt`
* Forcefully remove a directory named "old_documents" and all its contents:
`rm -rf `old_documents`

## Rmdir
### Definition: 
Removes empty directories.
Usage: rmdir directory_name
### Example:
* Remove an empty directory named "temp":
`rmdir temp`
* Remove multiple empty directories named "dir1", "dir2", and "dir3":
  `rmdir dir1 dir2 dir3`
* Remove a directory named "empty_folder" with a space in its 
`rmdir "empty folder"`

## Mv
### Definition: 
Moves or renames files and directories.
### Usage: 
`mv source destination`
### Example:
* Move a file named "document.txt" to the "documents" directory:
`mv document.txt documents/`
* Rename a file named "oldfile.txt" to "newfile.txt":
`mv oldfile.txt newfile.txt`
* Move all text files from the current directory to a directory named "text_files":
`mv *.txt text_files/`

## Cp
### Definition: 
Copies files and directories.
### Usage: 
`cp source destination`
### Example:
* Copy a file named "image.jpg" to a backup directory:
`cp image.jpg backup/`
* Copy a directory named "photos" and all its contents to a backup location:
`cp -r photos/ backup/`
* Copy multiple files named "file1.txt", "file2.txt", and "file3.txt" to a directory named "archive":
`cp file1.txt file2.txt file3.txt archive/`

## File
### Definition:
Determines the type of a file.
### Usage: 
`file file_name`
### Example:

* Determine the type of a file named "image.png":
`file image.png`
* Check the type of a binary executable named "program":
`file program`
* Identify the type of a compressed file named "archive.zip":
`file archive.zip`

## Pdfinfo
### Definition: 
Provides information and metadata from PDF files.
### Usage: 
`pdfinfo file_name.pdf`
### Example:
Get information about a PDF file named "document.pdf":
`pdfinfo document.pdf`
Check the number of pages in a PDF file named "presentation.pdf":
`pdfinfo presentation.pdf | grep Pages`

## Mediainfo
### Definition:
Provides technical and tag information about multimedia files.
Usage: 
`mediainfo file_name`
### Example:
* Get technical details about a video file named "movie.mp4"
`mediainfo movie.mp4`
* Check the duration of an audio file named "song.mp3":
`mediainfo song.mp3 | grep Duration`

## Exiv2
### Definition: 
Manipulates image metadata.
### Usage:
`exiv2 file_name`
### Example:
*View metadata information of an image file named "photo.jpg":
`exiv2 photo.jpg`
* Extract the camera model from an image file named "pic.jpeg":
`exiv2 -g CameraModel pic.jpeg`
* Remove all metadata from an image file named "image.png":
`exiv2 rm image.png`

## Exiftool
### Definition:
Reads, writes, and edits metadata in various file types.
### Usage:
exiftool file_name
### Example:
* Display all metadata information of an image file named "photo.jpg":
`exiftool photo.jpg`
* Edit the description tag of an image file named "pic.jpeg":
`exiftool -Description="New description" pic.jpeg`
* Extract GPS coordinates from an image file named "image.png":
`exiftool -GPSLatitude -GPSLongitude image.png`