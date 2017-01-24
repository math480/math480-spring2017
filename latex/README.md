# LaTeX Information

## How To Typeset your work in this class

You are strongly encouraged to use the 
[LaTeX document preparation system](http://www.latex-project.org/).  If you
don't already know how to use [LaTeX][], there is
[plenty of online documentation](#latex-resources) to help you get started, but
please *feel free to ask me if you need help!*  At the bottom of this page are
some [links to LaTeX resources](#latex-resources). 


If you ever have any trouble using [LaTeX][], please let me know! I am happy to help.
You can [send email](mailto:williamdemeo@gmail.com), or post a question
on Piazza.  You could also create a
[new wiki page](https://github.com/math480/math480-spring2017)
for discussing some topic, or open a [new issue](https://github.com/math480/math480-spring2017).

## Creating your first LaTeX document

Here is my usual workflow.  I will assume you have [LaTeX][] properly installed
on your computer.  (For installation instructions, see the links below.)

1. First I open up an existing LaTeX file in my editor of choice (which happens
   to be emacs).  (I never start from scratch because it's too hard to remember 
   all the LaTeX style and formatting commands that I typically like to use, and
   it's pointless to retype them all every time I start a new project.)

2. Next, I edit the file and add some content, and then I am careful to save the
   file under a new name, so I don't overwrite the file I started from!
   Let's call this new file `mypaper.tex`.

3. Next, I switch over to a terminal window and, on the command line, I switch
   to the directory containing the file `mypaper.tex`, and then I invoke the
   following command:
   
        pdflatex mypaper.tex

   Typically, I run this command at least twice.  The `pdflatex` program
   compiles my LaTeX source code, contained in the file `mypaper.tex`, and
   (assuming there were no errors) produces a pdf file called `mypaper.pdf`.

4. I open the file `mypaper.pdf` in a pdf viewer and inspect the contents.

The paper is almost never finished after the first compile.  Instead, I
typically repeat steps 2 and 3 a few hundred times before I'm satisfied.

## Storing your masterpiece in a Github repository
Of course, after a couple of hours, I'll want to be sure my hard work is
recorded until the end of time, so I add the `mypaper.tex` file 
(and possibly the .pdf file) to a local git repository, and then I push my 
changes to a remote repository on Github.  I carry out these steps as 
follows: 

Let's say I am in the `myproject` directory, which contains
`mypaper.tex`. To initialize the repository and add `mypaper.tex` to it, I do
the following on the command line:

    git init
	git add mypaper.tex
	git commit -m "initial commit of my masterpiece-in-progress"
	
Then I go to Github.com, login to my Github account, and create a new repository
called, say, `myproject`.  Then, back on the command line, I type:

    git remote add-url origin git@github.com:williamdemeo/myproject.git
	git push -u origin master
	
Luckily, you don't have to remember the last two commands because Github kindly
displays them everytime you create a new repository.
	
Please give this process a try.  I think you will find it's not too hard to get
the hang of it and, before you know it, you will have all your work nicely
archived on the web... so that it may have a broad, profound, and lasting impact
on all humankind.
	

## LaTeX Resources

+ **Using LaTeX in a browser**
  - [ShareLaTeX](http://www.sharelatex.com)
  
+ **Downloading/Installing LaTeX**
  - [General Information](https://www.latex-project.org/get/)
  - [TeXLive](http://www.tug.org/texlive/) is for Linux users.
  - [MacTeX](http://www.tug.org/mactex/) is for Mac users.
  - [proTeXt](http://www.tug.org/protext/) is for Windows users.

+ **Using LaTeX**
  - [LaTeX project site](http://www.latex-project.org/)
  - [LaTeX WikiBook](https://en.wikibooks.org/wiki/LaTeX)
  - [The not-so-short guide to LaTeX](http://mirror.ctan.org/info/lshort/english/lshort.pdf)
  - [George Gratzer's short course](http://www.ctan.org/tex-archive/info/Math_into_LaTeX-4/)
  - [Introduction to Using TeX](http://www.math.harvard.edu/texman/texman.html) (Harvard)
  - [TeX resources](http://www.ams.org/publications/authors/tex/tex) (American Mathematical Society)
	
+ **Using LaTeX for presentations (Beamer)**
  - [Beamer tutorial (uncg)](https://www.uncg.edu/cmp/reu/presentations/Charles%20Batts%20-%20Beamer%20Tutorial.pdf)
  -	[Beamer tutorial (mit)](http://web.mit.edu/rsi/www/pdfs/beamer-tutorial.pdf)

+ **Finding Math Symbols**
  - [Comprehensive Symbol List](http://mirrors.ctan.org/info/symbols/comprehensive/symbols-letter.pdf)
  - [Brief Symbol List](http://www.artofproblemsolving.com/Wiki/index.php/LaTeX:Symbols)
  - [Cheat Sheet (pdf)](http://ctan.math.washington.edu/tex-archive/info/latexcheat/latexcheat/latexsheet.pdf) [(html)](http://web.ift.uib.no/Teori/KURS/WRK/TeX/symALL.html)
  - [detexify][] If you can draw the symbol with your mouse, try [detexify][]!

+ **LaTeX Resources for Mac Users**
  - [Installing LaTeX on Mac OSX](http://www.howtotex.com/howto/installing-latex-on-mac-os-x/)
  - [MacTeX](https://tug.org/mactex/)
  - [TeXShop](http://pages.uoregon.edu/koch/texshop/)
  - [TeXworks](http://www.tug.org/texworks/)
  
Lots more links at: http://www.tug.org/begin.html

---------------------------------------------------------

## Text Editors

1. [Emacs](https://www.gnu.org/software/emacs/) (my favorite, but it's a
   heavy-weight; you might say it includes the kitchen sink)
   
2. [Vim](http://www.vim.org/) (what the "cool" kids are using these days)

For more options and opinions about text editors, see
http://lifehacker.com/five-best-text-editors-1564907215

Emacs is my favorite editor, and I highly recommend it. But beware, some people think it's very
challenging to learn to use emacs effectively. The diagrams below depict
alleged learning curves for various editors.

![learning curves](http://mrozekma.com/editor-learning-curve.png)

(more fake learning curves [here](http://www.manuelmagic.me/geek/texteditors/files/text_editors.jpg))





[A Beginner's Guide to LaTeX]: http://www.cs.princeton.edu/courses/archive/spr10/cos433/Latex/latex-guide.pdf
[LaTeX Guide]: http://en.wikibooks.org/wiki/LaTeX
[detexify]: http://detexify.kirelabs.org/classify.html
[LaTeX]: http://www.latex-project.org/
