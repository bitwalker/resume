## My Resume

This repository contains the TeX source for my current resume, as well as the most currently rendered PDF. You will find the source for the document structure in `resume.tex`, and the document styling in `schoens-cv.cls`. The rendered PDF will always be up to date with the source.

If you have any questions, or my resume has caught your eye for one reason or another, feel free to reach out to me via email, and I'll respond as soon as I'm able.

## Generating the PDF

There are several ways to generate a PDF from the Latex sources:


#### Using ShareLatex (no need to install any software)

[ShareLatex](http://www.sharelatex.com) is a web application for creating
and collaborating on LaTeX documents.  They have a free account that
can be used to compile this resume.

To get this resume compiled into a PDF with ShareLatex:

  1. Go to [sharelatex.com](http://www.sharelatex.com) and create first an account and then a project.
  2. In your new project replace the content of the `main.tex` file with the LaTeX source of resume's content (`cies-breijs-resume.tex` in this case) from Github.
  3. In your new project create a new file `resume.sty` and copy-paste
     the content of the same named file from the Github repo.
  4. Finally hit the "Compile" button to view and/or download the resulting PDF.

The result will be nice, but IMO will be nicer if you change the
rendering engine to XeLaTeX -- you can do so from the projects 'Setting' form
which hides behind the gear-icon on the left.

*TIP:* In the 'User Settings' (under 'Account' menu in the top-right) form you can set the spell-check language.


#### Using XeLaTeX

XeLaTeX is a version of Latex with great font rendering fuctionality (unicode, bidi,
special font features).  Since my resume uses 'lower case numerals' it
looks slightly better with XeLaTeX.

In recent Ubuntu versions you simply clone this project, change
directory to the root of the project and do:

        sudo apt-get install texlive-xetex texlive-latex-recommended tex-gyre
        ./xelatex *-resume.pdf

If all went well an updated version of the PDF is found in your current
working directory, alongside a bunch of `.log` and `.aux` files that
you can safely ignore.


### Using pdfLatex

Follow the same steps as for XeLaTeX, just replace the `./xelatex`
command with `./pdflatex`.
