# The Git and Bash Cheatsheet
Provides a number of useful commands concerning project management with a bash command line.

## Bash
### Basic Movement
Command | Usage
--------|--------
`pwd` | Shows the path to the current directory
`ls <dir>` | Lists the contents of a directory (default is `./`)
`cd <dir>` | Changes the directory to the given (`../` is alway the directory above,  `~/` is the contents of `$HOME` usually `/home/<username>`)

### File Management
Command | Usage
--------|------
`mkdir <dirname>` | Creates an empty directory.
`touch <filename>` | Creates an empty file.
`cat <file>` | Lists the input of the file.
`cp -r <dir> <dirname>` | Copies a directory and its content to `<dirname>`.
`cp <file> <filename>` | Copies a file to `<filename>`.
`mv <file/dir> <filename/dirname> `| Renames/Moves file or directory. 
`rm -r <dir>` | Deletes directory.
`rm <file>` | Deletes file.