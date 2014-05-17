# bash scripts

Some useful shell scripts I wrote over the years

## LaTeX and bibtex management

* <bib2bibclean> is a simple wrapper around *bib2bib* that removes any personal bibtex information and annotations such as Mendeley notes and tags, owner, timestamps, keywords, comments, summary or review fields. Handy for whenever you want to pass (some of your) richly annotated bibtex library on to other people.
* <extract-references> takes a LaTeX .aux file, extracts all references cited in the LaTeX document and puts them in a new references.bib file, stripping off annotations with *bib2bibclean* above. Practical when you only want to submit the relevant entries of a central large .bib file when making a submission in .tex/.bib format.
* <mybib2html> uses *bib2bib* to get all your own publications (filtered by author name) out of a .bib file and prints them out on two minimalist HTML files (a nicely decorated bibliography with links to the other file containing copy-paste-able bibtex entries) using *bibtex2html*. I use it to generate the publication list over at [my website](http://kevinstadler.github.io/)
* <wclatex> is a python script that gives the wordcount of a LaTeX document according to the regulations of the standard University of Edinburgh MSc Dissertation format (footnotes, tables, captions etc excluded from wordcount). This code formed the basis for my [LaTeX word count plugin for SublimeText](https://github.com/lionandoil/SublimeLaTeXWordCount)

## Audio processing scripts

* <rip> rips audio tracks off a CD and converts them to [flac](https://xiph.org/flac/) format, including metadata retrieval. It requires tools from the debian packages *cdparanoia*, *libcddb-get-perl* and *flac*.
* <tomp3> converts a flac file into an mp3 while preserving all tags. Requires *flac* and *lame*.
* <dirtomp3> uses *tomp3* to convert a directory of flac files, putting the output in a parallel directory.
