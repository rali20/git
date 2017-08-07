# Practise 
Here I am going to write some of the commonly used commands in git
# Help
* man git-<verb>
* git help <verb>
* git <verb> --help
# At the time of initiation of repository
* git config --global user.name "<username>" 
* git config --global user.email "<emailAddress>"
(By default the option is --local)
* git init
(To initialize your present working directory)
# To see the status of the repository
* git status
* git log
(To see the change log or the history of the project)
# Track files
* git add <file or directory>
(Adds file or directory to staging area, if just included with -A option it adds all files in working directory)
* git commit -m "<message>"
(Take a snapshot of project with staged files) 
# Branches
* git branch <branchName>
(To branchout to new one from the current one)
* git checkout <branchName>
(To start working in specified branch)
# Git ignore
(You can add filenames or patterns to ignore them while tracking them)
