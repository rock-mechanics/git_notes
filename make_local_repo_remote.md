# make local repo connected to github

# prerequisite
1. local repo is ready
2. github account is ready

# steps
## step 1 : create
* create a empty repo in github
* the repo can be any name

## step 2 : connect
* connect local repo to remote repo
* copy the ssh/https url from the github repo
* navigate to local git repo
* run `git remote add origin <url>`
* verify `git remote -v`

