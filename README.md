loriaprint
==========

This very simple script aims at fixing PDF that cannot be printed on the
LORIA printers (due to missing fonts, unsupported PDF features, etc.).

Usage
-----
fixpdf PDF_FILE

Some options are available, see fixpdf -h

Requirements
------------
This script uses pdftk, pdfinfo (from poppler-utils), and pdfnup (from texlive-extra-utils)
On Debian: apt-get -y install pdftk poppler-utils texlive-extra-utils
