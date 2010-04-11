# Slides

These are all files needed to typeset the slides used in the course. To typeset on of the lectures, you need:

* kursheader.tex (contains everything to typeset the slides)
* beameranpassungen.tex (eye candy)
* a file starting with a number (e.g. 01-Einführung und grundlegende Bedienung.tex)

Now, just say

    xelatex 01-Einführung und grundlegende Bedienung.tex

and you should get a nice pdf.

To compile all slides for every lecture at once, use the file einführungskurs2010.tex in the following way:

    xelatex --shell-escape einführungskurs2010.tex

This is a little misusing of TeX as script file, but it does it’s job.

## Renaming of a File

Be careful if you want to rename a file. There some heavy TeX hackery done to read the number and the title out of the name of the file. So don’t expect anything to work when changing filenames. Also, if you change anything in one of the other files, everything might collapse and your computer may turn into a black hole.
