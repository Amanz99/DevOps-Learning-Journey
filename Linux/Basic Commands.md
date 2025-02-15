# Basic Linux Commands

This file contains some of the most frequently used Linux commands that help us naviagate throughout our linux system.

## File and Directory Management

### `pwd`
- **Description**: Prints the current working directory

### `ls`
- **Description**: Lists files and directories in the current directory
- **ls -l**: Detailed Listing With Permissions
- **ls -a**: List all files including hidden files(files starting with .)

### `cd (Directory)'
- **Description**: Changes current Directory
- **cd .. **: Go up one directory
- **cd ~ **: Go to the home directory

### `touch (File name)` 
- **Description**: Creates an empty file (Updates the timestamp of an existing file)
- **touch newfile.txt**: Creates a new empty file named newfile.txt
- **touch file1.txt file2.txt**:  # Creates multiple files at once
- **touch -t 202502150800 file.txt**:  # Updates the timestamp to a specific date and time

### `mkdir` 
- **Description**: Creates a new directory.
- **mkdir new_folder**: Creates a new directory named new_folder

### `rmdir` 
- **Description**: Removes an empty directory
- **rmdir empty_folder**: Removes directory named Empty_folder

### `rm` 
- **Description**: Removes files or directories
- **rm file.txt**: Remove file named file.txt
- **rm -r folder/**: Remove a directory
- **rm -f file.txt**: force removal

### `cp` 
- **Description**: Copies Files or Directories
- **cp file.txt /path/destination/**: copies 'file.txt' to the specified destination directory
- **cp -r folder/ /path/destination/**: Recursively copies the 'folder' and its contents to the destination

### `mv` 
- **Description**: Moves or renames files and directories
- **cp file.txt /path/destination/**: Moves 'file.txt' to the specified destination directory
- **cp -r folder/ /path/destination/**: Renames 'old_name.txt' to 'new_name.txt'


