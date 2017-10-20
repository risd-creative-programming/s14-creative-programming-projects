## Week 1 - Feb 17: Workshop 1
## Getting Started with Git and GitHub

### 1. Prerequisites
* Install Git: [Getting Started Installing Git](http://git-scm.com/book/en/Getting-Started-Installing-Git)
    * [Installing on Mac](http://git-scm.com/book/en/Getting-Started-Installing-Git#Installing-on-Mac)
    * [Installing on Windows](http://git-scm.com/book/en/Getting-Started-Installing-Git#Installing-on-Windows)
    * [Installing on Linux](http://git-scm.com/book/en/Getting-Started-Installing-Git#Installing-on-Linux)
* Get Github account: [http://www.github.com](http://www.github.com)
* Sign up for free education account: [https://education.github.com/](https://education.github.com/)

### 2. Introduction to the Command Line
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

### 3. How Git Works
**Git** is a **versioning system** for files and software code.  This means it is a server that helps you store, track changes to and delete files as you work on them.  It is ideal for large collaborative teams working on a single project, since it helps to manage incoming changes from everyone in one single place.  It is also useful for single users who want to store their files somewhere with a full history of changes in order to **revert** to changes if files are ever lost.  A single git project is called a **repository** (or **repo** for short).

**[GitHub](http://www.github.com)** is a website that offers free git server space for individual and collaboration use.  If you want your git repos to be private, you can sign up for a [free education account](https://education.github.com/).  GitHub is also a social network, where you can find other people's git repos and follow, star, and even download (or fork/clone) other people's repositories so you can collaborate on them.  GitHub is **not** used to host websites or HTML files, just raw code or files to be tracked and maintained.

### 4. Getting Started with Git
* [Getting Started with Git](http://try.github.io/levels/1/challenges/1)
* Common git commands [Git command cheat sheet](http://www.git-tower.com/blog/git-cheat-sheet-detail/)
    * `git clone`
    * `git status`
    * `git add`
    * `git commit`
    * `git push`
    * `git pull`

![](http://i.imgur.com/66NShs3.png)


### 5. Fork Your First Repo
* At some point you may find yourself wanting to contribute to someone else's project, or would like to use someone's project as the starting point for your own. This is known as "forking".
* What is the difference between fork and clone?
* https://help.github.com/articles/fork-a-repo
* Fork a repo, clone it, make a change and create a pull request!

![](http://i.imgur.com/OcLcCCh.png)  
from [git simple guide](http://rogerdudler.github.io/git-guide/)

### 6. Create Your First Repo
* https://help.github.com/articles/create-a-repo
* Fill out form at: https://github.com/new

### 7. Advanced: More About GitHub Repos
* Example repository: [p5.js repository](https://github.com/lmccart/p5.js)
    * branches
    * issues
    * histories
    * blame
    * contributor list

### 8. More Resources
* [list of tutorials](https://help.github.com/articles/what-are-other-good-resources-for-learning-git-and-github)
* [git simple guide](http://rogerdudler.github.io/git-guide/)
* [github guides](http://guides.github.com/)
* 


### STEP BY STEP: Add your local changes to your github repository.

1. In Terminal, navigate to the folder where your project is located. (See "Introduction to command line" above)
2. To see the status of all the files that have been modified since your last commit, type:

  ```
  $ git status
  ```
3. "Stage" all the modified files (add them to your local .git):
  
  ```
  $ git add *
  ```
  You can also add them individually by typing each one by one:
  
  ```
  $ git add index.html
  $ git add package.json 
  // etc
  ```
  
4. Commit your changes with a message to ready all of your files for sending to github. Fill in the message with something useful.

  ```
  $ git commit -m "<your message here>"
  ```
5.  Push your changes to the web (github):
  
  ```
  $ git push origin master
  ```
  
6. If you refresh your github repo page online, you should see your updated files appear.

###STEP BY STEP: Syncing up your repository with the web

At some point, for example if you are collaborating with others, you may have changes in your github repository (remote repo) that you want to get into the copy of the code on your machine (local repository).

1. In Terminal, navigate into the folder of your project/repository.
2. Get the changes from the remote repo into your local repo:

  ```
  $ git pull origin master
  ```
  
3. If there are any conflicts, Terminal will let you know the line numbers and files where these occurred. You can open them with a text editor and manually resolve any problems.
