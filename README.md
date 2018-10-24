# GitHub Tutorial

_by Samara Fernandez_

---
## Git vs. GitHub
* Git is a version control which means it keeps snapshots of all your code, so that you can be able to look back at your old code. (It doesn't require github)
* Github stores code into the cloud. You can track your changes easily and you can collaborate on files. (It does require git)
  *  It runs in the command line and it's basic workflow which means you have a directory in where you can initialize git and call it a repository.


---
## Initial Setup
* Go to [github](https://github.com/)
* With making a github account, if you're a HSTAT student then use your Hstat email to create it, but if you're not then use an email you regularly use. 
  * After this, you should end up pressing free account and making your first repository
 
  
---
## Repository Setup
* With `git init`, you're initializing git in your repository
  * _Its like hiring a photograther_
* Then you do `git add file`  to add your files to the stage to be  commited
  * _Like adding people to a photo_
* After adding your file, you want to do `git commit -m "write your message here"`, this takes a 'snapshot' of your files and the message should describe what you did to your file
  * _Takes a photo_ 
* Now that you've added and committed, you're going to need somewhere to have all your work and this is where github comes in. You go to your github account and press the + on the left side opf your profile and then press on New Repository.You name your new repository the same name as your file, so that you can save all your work there. Once you press create, something that says Quick Setup will appear and you'll need to go to the second box that says '... or push an existing repository from the command line' and copy the two things into your file, but do them seperatly. (Make sure that in github on top you have it put as SSH)
* Now with the remote, it's so that we have a connection between our current repository and an external on


---
## Workflow & Commands
1. Git `status` is an optional command to see which files have been edited since the last command (they will be red) and which have been committed to the stage (they will be green).
2. With git add, there are three different ways you can use it. First way is with `git add file` which adds the files to stage to be committed. The second one is `git add .` which shortcut adds the current directory and all files have changes. The last one is `git add --all`which includes all changes, even deleted files.
3. `Git commit -m "message"` takes a ‘snapshot’ of the files on the stage. The message should describe what you did or fixed in your code(takes photo)
4. There's two ways to use git push. First, you use `git push - origin master` to send your commits to the remote and the -u makes git remember which repo to push the changes to and origin is the remote you're pushing it to. But if you've already done `git push -u origin master`then you can do `git push` which brings any changes from the remote down to the local



---
## Rolling Back Changes
1. To undo `git edit`, you do `git checkout -- filename`
2. To undo `git add`, you do `git reset HEAD filename` so yhat you can go back before you added the changes
3. To undo `git commit`, you do `git reset --hard HEAD~1` so that you can end up adding more things to your repo
4. To undo `git push`, you do `git push -f origin last_known_good_commit:branch_name`

 