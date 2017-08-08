## Practise 
Here I am going to write some of the commonly used commands in git

# Help
* man git-[verb]
* git help [verb]
* git [verb] --help

# At the time of initiation of repository
* git config --global user.name "[username]" 
* git config --global user.email "[emailAddress]"
(By default the option is --local)
* git init
(To initialize your present working directory)

# To see the status of the repository
* git status # using option -s will show in short 
* git log # using -p -2 will show code difference introduced in each commit 2 lines in each commit
* git log --stat # will show stats by file wise in numerals
(To see the change log or the history of the project)
* git log --pretty=format:"%h - %an, %ar : %s"
(Shows log in format specified)

# Track files
* git add [file or directory]
(Adds file or directory to staging area, if just included with -A option it adds all files in working directory)
* git reset HEAD [fileName]
(To unstage the adding)
* git commit -m "[message]"
(Take a snapshot of project with staged files, adding -a will skip staging of all files) 
(! To add some forgotten thing to latest commit)
* git add [fileName]
* git commit --amend
(To unmodify the changes before staging)
* git checkout -- CONTRIBUTING.md

# To remove files 
* git rm [fileName]
(Removes file from repository and needs to be commited)
* rm [fileName]
(Removes file from directory but needs to be staged )
* git rm --cached [fileName]
(Removes file from tracking-[from staging or commited] but is still present in directory)

# To check differences
* git diff [file]
(Shows the difference between staged and modified file, if you add option --staged; then it shows the difference between staged and the last commit)

# Branches
* git branch [branchName]
(To branchout to new one from the current one)
* git checkout [branchName]
(To start working in specified branch)

# Git ignore
* For that create a new file called .gitignore and add , for detail see gitignore command
(You can add filenames or patterns to ignore them while tracking them)

# Other commands
* git mv [oldName] [newName]
