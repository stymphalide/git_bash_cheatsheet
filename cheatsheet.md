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


## Git
### Basic File Tracking
Command | Usage
--------|------
`git init` | Initialises an empty git repository into the current directory.
`git status` | Shows the satus of the working directory. (Really verbose, great to decide what to do next.)
`git add <file>` | Adds the given file to the staging area
`git commit (-m <CommitMsg>)` | Adds the staged files to the repo, if the `-m` flag is omitted, the default editor will open.
`git log` | Shows every commit done.
`git checkout <file>` | Resets the contents of a file to the latest commit.
`git reset <Hash/Tag>` | Resets the contents of the directory to the state of the hash

### Branching
Command | Usage
--------|------
`git branch (-r)` | Shows all branches. The `-r` flag shows remote branches.
`git checkout (-b) <branchname>` | Switches (or creates) a branch with name `<branchname>`.
`git merge <branch>` | Merges `<branch>` with the current branch.
`git branch -d <branch>` | Deletes the branch.
`git branch --track <branch> <remoteBranch>` | Creates a branch that tracks a remote one.


### Working with Remotes
Command | Usage
--------|------
`git clone <link>` | Clones the repository from the `link`.
`git push <remote> <branch>` | Updates the remote branch.
`git fetch` | Updates local repository from remote.
`git pull <remote> <branch>` | Like `fetch` and `merge <remote> <branch>` combined.