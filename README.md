loriaprint
==========

This very simple script aims at fixing PDF that cannot be printed on the
LORIA printers (due to missing fonts, unsupported PDF features, etc.).

Usage
-----
Transform PDF into something that is suitable for printing even on broken printers:

    fixpdf PDF_FILE

Transform PDF and print it:

    export FIXPDF_SERVER=cups-nge.inria.fr
    export FIXPDF_PRINTER=printer-bw-nge
    export FIXPDF_USER=jdoe
    fixpdf -p PDF_FILE

Some options are available (for n-up, ranges, etc.), see fixpdf -h

Requirements
------------
This script uses pdftk, pdfinfo (from poppler-utils), and pdfnup (from texlive-extra-utils)

On Debian: apt-get -y install pdftk poppler-utils texlive-extra-utils
