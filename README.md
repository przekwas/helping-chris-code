# Helping Chris

### Things to download
1. [VS Code](https://code.visualstudio.com/) will be your editor of choice.  It is supported by Microsoft and has widespread developer support, and can be customized with cool extensions that I can show you later.  Compatible on Mac and Windows.  Autofill syntax, good error handling, and dark themed.  :)

2. (Windows Only) [Cmder](http://cmder.net/) will be replacing Command Prompt and Powershell outside of very niche scenarios.  It emulates a Unix bash style terminal that will give you all the commands you need to become a l337 coder.  If you're coding on Mac, the default terminal works just fine.
	* It does not have an installer exe, instead unzip it to a directory called "Cmder" on your harddrive.  And you're going to want it on the root or close to it if possible.  My PC at home is literally `C:/Cmder` as it'll make it easy to navigate around in your terminal from there instead of a path like `C:/Users/ChrisSmith/My Documents/NOT_PORN/furry/futanari/yiffing/boofing/Cmder`
	* Open a Command Prompt as an Administrator
	    -   Hit the Win key and type "CMD"
	    -   Right-click on "Command Prompt" and click "Run as Administrator"
	* Navigate to the directory you have placed Cmder
	    -   Use  `cd <directory>`  to get to the folder
	    -   For example: if you have the  `Cmder.exe`  in  `C:\Cmder`  you would type  `cd C:\Cmder`  and press  `Enter`
	* Execute this command:  `.\Cmder.exe /REGISTER ALL`
	    -   _If you get a message "Access Denied" ensure you are executing the command in an  **Administrator**  prompt._
	 * In a file explorer window right click in or on a directory to see "Cmder Here" in the context menu. From this point forward you can do this any time you need to open a command prompt.
	 
3. Download [git command line tools](https://git-scm.com/downloads).  You don't care about any of the frill on the install, just need the command line tools, no gui, no other bullshit.  Text me if there's anything you're not sure about.
	* Type `git --version` into your Cmder after installation (note you might need to close / reopen Cmder) and make sure you get a version response 
	* `git !== github` they are two separate things.  Github is an online "cloud" of sorts that will backup your code.  `git` is a command line tool to help link your local directory of code, to Github.  It allows you to pull new code, clone my repositories, make changes locally, and push to them up to the cloud
	* [Register for a Github account](https://github.com/) if you haven't already at this point.  It's free.  Remember your email, username, and password as you'll need to enter those into `git` tools the first time you push code, after which it'll remember your settings
	
---
That's it.  You're done.  You have all the beginning tools to start practicing coding.

--- 

### Command Line 
[Command Line Cheat Sheet](https://www.git-tower.com/blog/command-line-cheat-sheet/).  If you don't have any experience in a unix bash terminal, this will give you a list of possible stuff you can do.  I want you to be familiar with:
| command | purpose |
|--|--|
| `cd` | to navigate directories on your harddrive |
| `ls` | to list files in the directory you're in |
| `mkdir` | to create a new directory with a name in the directory you're in |
| `pwd` | to print your current working directory path |
| `touch` | to create files with extension names from terminal |

## First Exercise
**Achieve the following in Cmder**:
1. Navigate to the your root directory `C:/`
2. Make a new directory called `source`
3. Inside `source`, create a new directory called `my-first-project`
4. Inside `my-first-project`, create a new file called `index.html` (the resulting path should be `C:/source/my-first-project/index.html`)
5. Use `code .` to open this directory in VS Code automatically

**Next Steps in VS Code**:

6. Using [emmet abbreviation](https://code.visualstudio.com/docs/editor/emmet) create a dope boilerplate for your HTML page  
	* *Hint*: You can literally type `!` at the top of your blank HTML page and hit `enter` and it will auto fill your basic head and body structure of an HTML page.
7. Add an `<h1>` that displays "Hello World!" in the body of your HTML code
8. Save the file

**Next Steps in Chrome**:

9.   While logged in on Github, go to your profile page and click on the repositories tab, and click the green `New` repository button.
9. Give it a repository name using lowercase and hyphens.  Kind of like your directory name, and note that it *does not* have to match your directory name, but it's typically good practice to do so
	* Description doesn't matter, Public, and we don't care about initializing with a readme 
10.  Copy the `https://github.com/przekwas/helping-chris-code.git` link from the `Quick Setup` field you'll see at the top.  Yours will obviously have your gituhb username and the repo name

**Next Steps in Cmder**: 

12. `pwd` to ensure you're in your `C:/source/my-first-project` directory
13. `ls` to ensure you have your `index.html` in this directory
14. Run `git init`, this will create a hidden git folder that will serve as the link between your local directory and its online repo.  It also tracks any changes you make that aren't in your online code
15. Run `git status` and it should show you in red text that `index.html` is an untracked file
16. Run `git add .` the single `.` represents *this* directory, so this command tells git to add **all** files and changes in this directory, you'll be using this 99% of the time at your level
17. Run `git commit -m "first commit"` this will add a message with your newly added/tracked files.  The `-m` is a required message flag, and for the love of god the message must be wrapped with `" "` otherwise you'll open VIM and fuck it all up.  Text me if you do, lol
	* commits are typically lowercase, using present progressive verbs, and short, ie "adding changes to my footer", "updating html file structure", etc 
18. Run `git remote add origin https://github.com/przekwas/helping-chris-code.git` where you paste **your** link you coped earlier instead of mine.  This connects your local git folder to the online repo you've created
19. Run `git push -u origin master` and this will push your added and committed code to your Github repo!  The `-u` is a flag that sets the upstream to a `master` branch which you'll be working out of.  Go refresh your Chrome page and you'll see your `index.html` has been successfully pushed to Github!!!!  Congrats!

## Second Exercise
**Back in VS Code**:
1. Wrap your `<h1>` with a `<div>` and give the wrapping div a class name of `boofing`
2. Save the file

**Next Steps in Cmder**:

3. Run `git status` and notice it detected changes in your `index.html` file
4. Run `git add .` to add all pending changes in this directory
5. Run `git commit -m "adding a wrapping div"` to commit this change with what we did
6. Run `git push` and you're all set!  It pushed our new code to your Github repo.  Refresh your Chrome page again and you'll see the new `index.html` with our new code in there

# Congrats!
You've achieved the first baby steps into a brand new world of development and you should be pretty fucking proud.  Text me your github repo link to show off your progress and I'll send you the next lab.  :) 

The first exercise taught you how to initialize a new project locally and and to connect it to an online repo, and do your first push to it.  The second shows you the method to push changes after the first push.  Since it's connected you won't need to add a remote or set an upstream.  

Below is the TL;DR for project set up and then pushing subsequent changes:

1. Any new lab or exercise I give you will be its own directory
2. `git init` in the new lab directory
3. `git add .`
4. `git commit -m "your message"`
5. `git remote add origin https://your-github-repo-link/`
6. `git push -u origin master`
7. After this initial setup, any changes you make in this directory will be added via
8. `git add .`
9. `git commit -m "your message"`
10. `git push`

1-6 for fresh projects, 8-10 for existing projects.  

 