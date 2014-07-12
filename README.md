#How to use git and github?
	Here all the steps and git bash code snippet are discussed shortly but effectively.

#1. to set name and email address for a repo
	git config --global user.name "mofassel"
	git config --global user.email "mofassel.me@gmail.com"

#2. To initiating git repo we need to create a directory where to set the local repo named gitrepo.git
	git init gitrepo.git
#3. when we create a file in gitrepo.git folder then we need to add it before making commit
	git add . or git add filename
	git commit -m "commit message here"
#4. We can see status or log message
	git status
	git log
#5. We can see difference with old file when their is a change
	git diff //before adding it using git add command
	git diff --cached //when it is already added/staged

#6. Shortcut for status, log and for speedy add+commit
	git staus -s
	git log --oneline
	git commit -a -m "commit message goes here" // it will directly add and commit. it must use with existing file that were commited before not very new file.

#7. when our log message will be larger than terminal screen then their will be appeared a message named "end" at the bottom of the screen
	shift+zz //We need to press shift+zz to be get rid of from here.

#8. To create and use ssh key follow this link
	https://help.github.com/articles/generating-ssh-keys

#9. Commands to connect your local repo with githup repo (either 1st one or 2nd one)
	git remote add origin your-github-project-ssh-url
	git remote add github your-github-project-ssh-url

#10. To upload/push local repo to github repo (note: origin = origin and github = github)
	git push -u origin master
	git push -u github master