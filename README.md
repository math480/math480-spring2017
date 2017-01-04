# Math 480 Spring 2017 -- University of Hawaii

This is the main repository and webpage for William DeMeo's section of Math 480.

If you have questions, comments, or suggestions, please open a [New Issue].

The url for this page is https://github.com/williamdemeo/math480-spring2017

## How To Typeset Your Papers and Slides

You must use the [LaTeX document preparation system](http://www.latex-project.org/).  If you
don't already know how to use LaTeX, there is
[plenty of online documentation](#latex-resources) to help you get started, but
please *feel free to ask me if you need help!*  At the bottom of this page are
some [links to LaTeX resources](#latex-resources). 


## How To Submit Your Work

**Overview**

You will use Git and GitHub to manage all of your work for this class.
Here are the steps you will follow to record and submit your work.

1. Sign up for a GitHub account (unless you already have one)
   at [github.com](https://github.com) and then 
   [email me](mailto:williamdemeo@gmail.com) immediately 
   to tell me your github username. 

2.  [Install Git](https://help.github.com/articles/set-up-git) on your computer.  

3.  If you are using a Mac or Linux, 
	[upload a public ssh key](https://help.github.com/articles/generating-ssh-keys)
    to your GitHub account. (If you are using [GitHub for Windows][] 
	you can skip this step.)

4. After I receive your github username, I will add you to 
   the GitHub organization called `math480`.

5. Once you are a member of `math480`, create a new repository (where you will 
   store all of your work for this class).  Make sure the "owner" of the
   repository is `math480`. **Important:** So that I can identify this
   repository as yours and give you credit for the work you do, be sure to name
   your repository with your last name followed by `-math480-spring2017`.
   For example, if your name is John Smith, name your repository, `smith-math480-spring2017`.

**Getting Help**

Please check out the
[5 Easy Guides to Help You Get Started](http://cjbrock.github.io/blog/2012/10/23/5-easy-guides-to-help-you-get-started-with-github/), especially if you are new to git.
In particular, the [15 minute Git tutorial][], the
[git--the simple guide][], and the [GitHub help pages][] are excellent.
For detailed comprehensive documentation see http://git-scm.com/doc.  
   
Do not be afraid to ask questions.  I am here to give you as much help as you
need to get started with git and Github.  Git takes a little time and practice 
to get used to, and I don't expect it to be easy. But I hope you will 
trust me that it can be an invaluable resource for managing projects and
collaborating with others.  If you stick with it, I believe you will be very
happy you did so. 
   

## Create your first repository (locally)

Here we will create a "local" respository that resides on your own computer.  
In the next section we will create a "remote" version of your repository 
in the cloud (i.e. on Github), and we will synchronize the two.

The steps below should work on **Mac** and **Linux** computers.

**Windows** users may try the
[GitHub for Windows][] app, but please note that 
I have never used it, so I won't be able to help if you get stuck.  
However, according to [this help.github.com page][], it's easy. 
If you have problems, please consult http://windows.github.com/help.html
See also the [first Tip](#git-tips) below.


**Creating a local git repository on the command line**

1. On your computer, open a terminal window, create a new directory to store
   your git repositories.
	
        mkdir -p ~/git

2. Initialize a new git repository inside your git directory:


		cd ~/git
		mkdir smith-math480-spring2017
		cd smith-math480-spring2017
		git init
		
3. Use your favorite editor to create a README.md file that gives a brief 
   description of your new repository. (Be very brief for now; you will add to it
   later.)
   
        cat >> README.md
		This is a repository of my work for Math 480.
		<ctrl-C>

4. Stage your changes

		git add README.md
		
5. Commit your changes to your local repository

		git commit -m "initial commit of README.md file"
		
    (In quotes is your comment explaining, if possible, *why* the
    changes were made.)
	
6.  Once you have set up your remote Github repository, [push][]
    your changes to the remote repository as follows: 

        git push origin master

    If you get errors, please let me know!  
	
	As soon as you push your changes to GitHub, they will be viewable by
    everyone.
	

## Git Tips
+ If you've set up Git and your GitHub account properly, you won't have to enter
your GitHub password every time you push changes to the repository. If you use a 
Mac or Linux, you should upload your public ssh key to your GitHub
account by following
[these instructions.](https://help.github.com/articles/generating-ssh-keys) In
Windows, this should work automatically if you use the
[native GitHub app](https://github-windows.s3.amazonaws.com/GitHubSetup.exe).

+ If you're a fan of Emacs, you might want to install the Emacs package called
[Magit][], which enables you to commit and push without leaving the Emacs
editor--very convenient!  ([Magit cheatsheet](http://daemianmack.com/magit-cheatsheet.html))
	
+ [This page][] on recording changes to the repository is extremely informative.
There is a lot of information on that page.  If you're new to version
controlling, don't be scared, we'll only need the very basics.
	
+ Optimally, your commit comments should indicate *why* changes were made, 
and not *what* was changed. Git keeps a perfect record of what was changed, so
comments mentioning this are somewhat redundant (although they can sometimes be
helpful).  Instead, try to give some justification of the changes.
This is often hard to do in just a few lines and without spending too
long thinking about each commit, so don't worry too much; just
keep it in the back of your mind.

+ If you ever have any trouble using Git or GitHub, please let me know!
You can [email me](mailto:williamdemeo@gmail.com) or open a [new issue](https://github.com/math480/math480-spring2017/issues/new).

## LaTeX Resources

+ **Downloading/Installing LaTeX**
  - [TeXLive](http://www.tug.org/texlive/) is for Linux users.
  - [MacTeX](http://www.tug.org/mactex/) is for Mac users.
  - [proTeXt](http://www.tug.org/protext/) is for Windows users.

+ **Using LaTeX**
  - [LaTeX project site](http://www.latex-project.org/)
  - [LaTeX WikiBook](https://en.wikibooks.org/wiki/LaTeX)
  - [The not-so-short guide to LaTeX](http://mirror.ctan.org/info/lshort/english/lshort.pdf)
  - [George Gratzer's short course](http://www.ctan.org/tex-archive/info/Math_into_LaTeX-4/)
  - [Introduction to Using TeX](http://www.math.harvard.edu/texman/texman.html) (Harvard)
  - [Some useful tips, esp. for Linux users](http://people.virginia.edu/~ll2bf/docs/quickref/latex.html) (Virginia)
  - [Video tutorials](http://www.spoken-tutorial.org/list_videos?view=1&foss=LaTeX&language=English)
	
+ **Finding Math Symbols**
  - [Comprehensive Symbol List](http://mirrors.ctan.org/info/symbols/comprehensive/symbols-letter.pdf)
  - [Brief Symbol List](http://www.artofproblemsolving.com/Wiki/index.php/LaTeX:Symbols)
  - [Cheat Sheet (pdf)](http://ctan.math.washington.edu/tex-archive/info/latexcheat/latexcheat/latexsheet.pdf) [(html)](http://web.ift.uib.no/Teori/KURS/WRK/TeX/symALL.html)
  - [detexify][] If you can draw the symbol with your mouse, try [detexify][]!

Lots more links at: http://www.tug.org/begin.html



[due date]: https://github.com/williamdemeo/Math700Homework/wiki/Homework-Schedule
[upload a public ssh key]: https://help.github.com/articles/generating-ssh-keys
[New Issue]: https://github.com/williamdemeo/Math700Homework/issues
[Clone]: http://git-scm.com/book/en/Git-Basics-Getting-a-Git-Repository#Cloning-an-Existing-Repository
[clone]: http://git-scm.com/book/en/Git-Basics-Getting-a-Git-Repository#Cloning-an-Existing-Repository
[install Git]: https://help.github.com/articles/set-up-git
[Fork]: https://help.github.com/articles/fork-a-repo
[fork]: https://help.github.com/articles/fork-a-repo
[pull request]: https://help.github.com/articles/using-pull-requests
[forks]: https://help.github.com/articles/fork-a-repo
[pull requests]: https://help.github.com/articles/using-pull-requests
[Commit]: http://git-scm.com/book/en/Git-Basics-Recording-Changes-to-the-Repository#Committing-Your-Changes
[commit]: http://git-scm.com/book/en/Git-Basics-Recording-Changes-to-the-Repository#Committing-Your-Changes
[Push]: https://help.github.com/articles/create-a-repo#step-3-push-your-commit
[push]: https://help.github.com/articles/create-a-repo#step-3-push-your-commit
[15 minute tutorial]: http://try.github.io/levels/1/challenges/1
[A Beginner's Guide to LaTeX]: http://www.cs.princeton.edu/courses/archive/spr10/cos433/Latex/latex-guide.pdf
[LaTeX Guide]: http://en.wikibooks.org/wiki/LaTeX
[Git--the simple guide]: http://rogerdudler.github.io/git-guide/
[GitHub help pages]: https://help.github.com/
[15 minute Git tutorial]: http://try.github.io/levels/1/challenges/1
[This page]: http://git-scm.com/book/ch2-2.html
[Magit]: http://magit.github.io/
[detexify]: http://detexify.kirelabs.org/classify.html
[GitHub for Windows]: https://help.github.com/articles/set-up-git#platform-windows
[this help.github.com page]: https://help.github.com/articles/adding-repositories-with-github-for-windows
