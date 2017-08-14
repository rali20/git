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

# Clone repository
* git clone [ssh,https url]

# Alias or Alternate names
git config --global alias.[aliasName] [command]

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
(To rename any file or directory)
* git tag # tags are used to mark important
(Lists the tags marked)
* git tag [tagName] # creates lightweight tag, it's just alais to commit
* git tag -a [tagName] -m "[message]"
(Used to create a tag)
* git show [tagName]
(Shows information about tag)
* git push [remoteName] [tagName]
(Pushes tags which are not by default not pushed, including just --tags pushes all)
# Remote Repository
* git remote 
(Gives list of remote repository(s), if included with -v gives details)
* git remote add [nameOfRemote] [ssh,https url] 
* git remote rename [oldName] [newName]
* git remote show [remoteName]
(Shows details about remote repository)
* git remote remove [repoName]
(Removes the server url)

# Fetch files (Does not merge to local)
* git fetch [remoteName])

# Push files
* git push [remoteName] [localBranch]
* 
