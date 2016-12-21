# kTheTex-bundle

The kTheTex-bundle is a collection of classes and packages to write
reports, theses etc. in LaTeX. The intention is to provide
comprehensive and out-of-the-box templates that are easy to use
without any need to include modifications, dozens of packages
etc. Most of the templates out there take convenience and technical
aspects over an elaborate design, these templates try to combine all
of that. Typographic rules are applied, always trying to stick close
to the suggestions given in literature. One of the major references
for these templates is *The Elements of Typographic Style* by Robert
Bringhurst.

Please feel free to suggest anything you would consider to be useful
for a report and/or thesis template as well. Or even start
contributing yourself!


## Is there a stable release?

Yes, there is. Although this bundle is still on a beta stage in terms
of its development, the
[latest release](https://github.com/knutzk/kTheTex-bundle/releases/latest)
can always be found on the
[release page](https://github.com/knutzk/kTheTex-bundle/releases/) of
this package.

There are still some points to be crossed from the to do list, before
everything goes to a stable v1.0 relase. If you are interested to try
the current code, simply download it!

The bundle is based on the docstrip utility, combing both
documentation and code in the same files. To get the the class and
package files, run LaTeX on the script `kTheTex-bundle.ins` by calling

```
$ latex kTheThex-bundle.ins
```
Then copy the output files to the base folder of your
project. Currently, the output files include:
- `ktxreprt.cls` -- a class to write reports
- `ktxthss.cls` -- a class to write theses
- `ktxbbltx.sty` -- a package for bibliography formatting (the
  functionality is included in the classes well, but this package can
  then also be used a stand-alone for other templates)

The writing of a documentation is still in progress and right now only
includes a commented version of the code. It can be generated by
running LaTeX/pdfLaTeX on the file `kTheTex-bundle.dtx` via

```
$ pdflatex kTheTex-bundle.dtx
```


## But how do those templates look like?

Although still on a very early stage, there are showcase files for the
classes `ktxreprt` and `ktxthss`. The code includes the `.tex` file
for both showcases, a compiled version is included in every release on
the
[release page](https://github.com/knutzk/kTheTex-bundle/releases/). To
compile them yourself, call

```
$ pdflatex showcase-report.tex
$ biber showcase-report
$ pdflatex showcase-report.tex
```

The program `biber` is needed since the generation of the bibliography
is done with the package Biblatex instead of the old BibTeX. Biblatex
and `biber` are part of every major TeX distribution and are available
as stable releases 2.0 and 1.0 since summer 2012, respectively. If you
haven't switched to Biblatex in your projects, you should consider it!
The main reason for this package to use Biblatex is the fact that its
style files are written in LaTeX code and are therefore much easier to
read, to understand and to adjust -- compared to files based on BibTeX
code which is painful to work with.


## To Do List

A list of open issues can be found on the
[github pages](https://github.com/knutzk/kTheTex-bundle/issues/). If
you have anything that should be added to these templates, suggestions
for improvement or bug fixes, you should check the list of open issues
first. If you can't find anything related there, feel free to open a
new issue yourself -- or submit a pull request, of course. :>
