===============================================
SASA Sentiment Analysis Tool
===============================================

Installation
===============

Pip Installation of library files
-------------------------------------

SASA tool can be installed with pip, the python module installer:

> pip install sasa

You may need to use `sudo` i.e.,

> sudo pip install sasa

see the python tool `virtualenv` for information about local installation.

You will also need to install nltk.  Please see the link below for instructions for NLTK.

Download source
-----------------

The source code for this tool can also be downloaded with git.  Simply check
out the code using git::

> git clone https://yourgoogleid@code.google.com/p/sasa-tool/

or if you don't have a google id::

> git clone https://code.google.com/p/sasa-tool/

Dependencies
----------------

This project depends on NLTK, the natural language toolkit, which also depends
on other libraries.  Please follow the instructions for installing this
library at http://nltk.org/install.html .
(windows users may need to consult http://selfsolved.com/problems/setuptools-06c11-fails-to-instal)


Usage
============

Note: these programs are designed to be run in a command line environment.
The usage instructions were designed for a linux environment, but should work
comparably in other posix type environments (e.g., mac terminal, cygwin on
windows)

Currently, the command line script is not installed system-wide, so follow the 
git source installation instructions.  The command line script is in ./bin

If the python library was not installed through `pip`, then the
sasa directory/folder must added to the python path::

> . setup.env

or::

> export PYTHONPATH=<path to directory containing this readme>

(Windows equivalent is : set PYTHONPATH=<path to this directory>)


Note: sentiment analysis is not for the faint of heart.  If you are easily
offended by vulgar language, please close your eyes and scroll down::

> echo -e "fuck this fucking shit\ngreat sounds good I love it" | ./bin/classifyFromCmdLine.py



License
============

This work is released under the `Apache 2.0 license
<http://www.apache.org/licenses/LICENSE-2.0>`_


Acknowledgements
==================

This code was first released by the collaboration of two labs at the
University of Southern California (USC), the Signal Analysis and
Interpretation Laboratory (SAIL) and Annenberg Innovation Laboratory (AIL).
The sentiment research at SAIL is supported by grants including NSF, NIH, and
DARPA.  The sentiment research at AIL is sponsored by the lab sponsors,
especially IBM, a AIL founding sponsor, and Orange, the flagship brand of
France Telecom.

This work was made possible by using existing open source projects and code.
NLTK (nltk.org) provides some of the basic classes of the SASA tool,
e.g. frequency distributions and classifiers.  Christopher Potts' twitter
specific tokenizer for sentiment analysis is used for tokenization. 

