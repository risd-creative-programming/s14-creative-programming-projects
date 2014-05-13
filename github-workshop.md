##Week 1 - Feb 17: Workshop 1
##Getting Started with Git and GitHub

###1. Prerequisites
* Install Git: [Getting Started Installing Git](http://git-scm.com/book/en/Getting-Started-Installing-Git)
    * [Installing on Mac](http://git-scm.com/book/en/Getting-Started-Installing-Git#Installing-on-Mac)
    * [Installing on Windows](http://git-scm.com/book/en/Getting-Started-Installing-Git#Installing-on-Windows)
    * [Installing on Linux](http://git-scm.com/book/en/Getting-Started-Installing-Git#Installing-on-Linux)
* Get Github account: [http://www.github.com](http://www.github.com)
* Sign up for free education account: [https://education.github.com/](https://education.github.com/)

###2. Introduction to the Command Line
The command line (or terminal) is a text-based way to navigate your operating system's files.  Instead of clicking through folders, you type commands to navigate folders, create and delete files, and much more.
* **Windows** [List of Windows commands](http://ss64.com/nt/)
  * Start the command line
      * Start > Run Command Line
  * List a folder's files
      * Type `dir` and press enter
  * Go to another folder
      * Type `cd` followed by folder name, and press enter
      * Type `cd ..` to navigate up one folder
  * Create an empty file in the current folder
      * Type `NUL > EmptyFile.txt`
* **OSX** [List of Linux/OSX commands](http://ss64.com/bash/)
    * Start the command line
        * Applications > Utilities > Launch **Terminal**
    * List a folder's files
        * Type `ls`
    * Go to another folder
        * Type `cd` followed by folder name, press enter
        * Type `cd..` to navigate up one folder
    * Create an empty file in the current folder
        * Type `touch EmptyFile.txt`

###3. How Git Works
**Git** is a **versioning system** for files and software code.  This means it is a server that helps you store, track changes to and delete files as you work on them.  It is ideal for large collaborative teams working on a single project, since it helps to manage incoming changes from everyone in one single place.  It is also useful for single users who want to store their files somewhere with a full history of changes in order to **revert** to changes if files are ever lost.  A single git project is called a **repository** (or **repo** for short).

**[GitHub](http://www.github.com)** is a website that offers free git server space for individual and collaboration use.  If you want your git repos to be private, you can sign up for a [free education account](https://education.github.com/).  GitHub is also a social network, where you can find other people's git repos and follow, star, and even download (or fork/clone) other people's repositories so you can collaborate on them.  GitHub is **not** used to host websites or HTML files, just raw code or files to be tracked and maintained.

###4. Getting Started with Git
* [Getting Started with Git](http://try.github.io/levels/1/challenges/1)
* Common git commands [Git command cheat sheet](http://www.git-tower.com/blog/git-cheat-sheet-detail/)
    * `git clone`
    * `git status`
    * `git add`
    * `git commit`
    * `git push`
    * `git pull`

![](http://i.imgur.com/66NShs3.png)


###5. Fork Your First Repo
* At some point you may find yourself wanting to contribute to someone else's project, or would like to use someone's project as the starting point for your own. This is known as "forking".
* What is the difference between fork and clone?
* https://help.github.com/articles/fork-a-repo
* Fork a repo, clone it, make a change and create a pull request!

![](http://i.imgur.com/OcLcCCh.png)  
from [git simple guide](http://rogerdudler.github.io/git-guide/)

###6. Create Your First Repo
* https://help.github.com/articles/create-a-repo
* Fill out form at: https://github.com/new

###7. Advanced: More About GitHub Repos
* Example repository: [p5.js repository](https://github.com/lmccart/p5.js)
    * branches
    * issues
    * histories
    * blame
    * contributor list

###8. More Resources
* [list of tutorials](https://help.github.com/articles/what-are-other-good-resources-for-learning-git-and-github)
* [git simple guide](http://rogerdudler.github.io/git-guide/)
* [github guides](http://guides.github.com/)
* 


### STEP BY STEP: Make a change to someone else's repository and submit a pull request!

#### Fork and clone and modify a repository (including first-time setup)
1. Go to the github page of the repo you would like to modify.
2. Click the "Fork" button in the upper right corner.
3. Copy the link in the box right below "Settings" in the right side menu. It should look something like: `https://github.com/risd-creative-programming/s14-creative-programming-projects.git`
4. On a mac, open Terminal (Applications > Terminal).
5. Navigate to the folder you'd like your project to be. (See "Introduction to command line" above)
6. Type `git clone https://github.com/risd-creative-programming/s14-creative-programming-projects.git`. You should see some output in Terminal indicating something is downloading.
7. Use Finder to go to the folder where you put the project, you should see the project files (ex: readme.md, etc).
8. Open these in any text editor and make your change, then save and close the file.
9. In Terminal, type `git status`. You should see a list of modified files.
10. Type `git add *` to add all modified files.
11. Type `git commit -m "<your message here>"` to ready all of your files for sending to github. Fill in the message with something useful.
12. Type `git push origin master` to push your changes to the web (github).
13. Back on github, go to the page of your github repository. Click the "Pull Requests" item in the right side menu.
14. Click the green "New Pull Request" button at the top of the page, and fill in the form, and submit. You're done!

####Syncing up your repository with the web
At some point, after your pull request and other changes have been made to the main repository, you might want to pull these changes into your own local copy again.

1. In Terminal, navigate into the folder of your project/repository.
2. Type `git pull origin master`. 
3. If there are any conflicts, Terminal will let you know the line numbers and files where these occurred. You can open them with a text editor and manually resolve any problems.
4. Repeat steps 10-14 above to push all sync'd changes to the web (github) again.
