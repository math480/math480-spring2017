# Storing and managing your projects with git and Github

You will use [git][] and [Github][] to manage your work for this class.
Here is a description of the steps you will take to get up and running
with git.

If you have any trouble with any of these steps, please notify your
instructor right away!
You can [send email](mailto:williamdemeo@gmail.com), or post a question on Piazza.
You could also open a [new issue](https://github.com/math480/math480-spring2017/issues/new).


## Setting up your Github account

1. Sign up for a Github account (unless you already have one)
   at [github.com](https://github.com) and then 
   [email me](mailto:williamdemeo@gmail.com) immediately 
   to tell me your github username. 

2.  [Install Git](https://help.github.com/articles/set-up-git) on your computer.  

3.  If you are using a Mac or Linux, 
	[upload a public ssh key](https://help.github.com/articles/generating-ssh-keys)
    to your Github account. (If you are using [Github for Windows][] 
	you can skip this step.)

4. After I receive your github username, I will add you to 
   the Github organization called `math480`.

5. Once you are a member of `math480`, on the [Github][] website, 
   create a new repository (where you will store all of your work for
   this class).  Make sure the "owner" of the repository is `math480`. 
   
   **Important:** So that I can identify this
   repository as yours and give you credit for the work you do, be sure to name
   your repository with your last name followed by `-math480-spring2017`.
   For example, if your name is John Smith, name your repository, `smith-math480-spring2017`.

   
--------------------------------------

## Create your first repository (locally)

In step 5 of the previous section, we created a remote repository
"in the cloud" (i.e. on Github).
Now we will create a "local" respository that resides on your own computer.
Finally, in the next section, we will see how to synchronize the local
and remote repositories, and learn how to [push][] and [pull][]
our changes from one to the other.

The steps below should work on **Mac** and **Linux** computers.

**Windows** users may try the
[Github for Windows][] app, but please note that 
I have never used it, so I won't be able to help if you get stuck.  
However, according to [this help.github.com page][], it's easy. 
If you have problems, please consult http://windows.github.com/help.html
See also the [Git Tips](#git-tips) below.


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
	
---------------
## Synchronizing local and remote repositories
We will now see how to synchronize the local
and remote repositories that you created in the previous sections, 
and learn how to [push][] and [pull][]
changes from one to the other.

After step 5 of the last section, your local repository should contain
a file called README.md.  Now we will see how to 
[push][] the contents of the local repository up to the remote repository.

1.  Go to the Github page for the remote repository you created
    above.  You should see instructions for connecting the local and
    remote repositories.  For example:
	
	    git remote add-url origin git@github.com:math480/smith-math480-spring2017.git
   
2.  If that command is successful, then we push the changes from local
    to remote as follows:

        git push -u origin master

    If you get errors, please notify your instructor right away!
	You can [send email](mailto:williamdemeo@gmail.com), or post a question on Piazza.
	You could also open a [new issue](https://github.com/math480/math480-spring2017/issues/new).
	
**Note:** As soon as you push your changes to Github, they will be viewable by everyone.
	
--------------------------------------

**Getting Help**

Please check out the
[5 Easy Guides to Help You Get Started](http://cjbrock.github.io/blog/2012/10/23/5-easy-guides-to-help-you-get-started-with-github/), especially if you are new to git.
In particular, the [15 minute Git tutorial][], the
[git--the simple guide][], and the [Github help pages][] are excellent.
For detailed comprehensive documentation see http://git-scm.com/doc.  
   
Do not be afraid to ask questions.  I am here to give you as much help as you
need.  Git takes a little time and practice 
to get used to, and I don't expect it to be easy. But I hope you will 
trust me that it can be an invaluable resource for managing projects and
collaborating with others.  If you stick with it, I believe you will be very
happy you did so. 

## Git Tips
+ If you've set up [git][] and your [Github][] account properly, you won't have to enter
  your Github password every time you push changes to the repository. If you use a 
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

+ If you ever have any trouble using [git][] or [Github][], please let your instructor know!
  You can [send email](mailto:williamdemeo@gmail.com), or post a question on Piazza.
  You could also create a [new wiki page](https://github.com/math480/math480-spring2017/wiki)
  for discussing some topic, or open a 
  [new issue](https://github.com/math480/math480-spring2017/issues/new).

--------------------------------------

[upload a public ssh key]: https://help.github.com/articles/generating-ssh-keys
[Clone]: http://git-scm.com/book/en/Git-Basics-Getting-a-Git-Repository#Cloning-an-Existing-Repository
[clone]: http://git-scm.com/book/en/Git-Basics-Getting-a-Git-Repository#Cloning-an-Existing-Repository
[Github]: https://github.com
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
[Github help pages]: https://help.github.com/
[15 minute Git tutorial]: http://try.github.io/levels/1/challenges/1
[This page]: http://git-scm.com/book/ch2-2.html
[Magit]: http://magit.github.io/
[detexify]: http://detexify.kirelabs.org/classify.html
[Github for Windows]: https://help.github.com/articles/set-up-git#platform-windows
[this help.github.com page]: https://help.github.com/articles/adding-repositories-with-github-for-windows
[git]: https://git-scm.com/

