
# Cocktail Shaker: Drug Expansion and Enumeration!
------------------------------------------------------------------------

![Build status](https://travis-ci.org/Sulstice/Cocktail-Shaker.svg?branch=master)
[![Coverage Status](https://coveralls.io/repos/github/Sulstice/Cocktail-Shaker/badge.svg?branch=master)](https://coveralls.io/github/Sulstice/Cocktail-Shaker?branch=master)
[![License](https://img.shields.io/badge/license-new%20BSD-blue.svg)](https://github.com/Sulstice/CocktailShaker/blob/master/LICENSE)
[![Join the chat at https://gitter.im/Cocktail-Shaker/community](https://badges.gitter.im/Cocktail-Shaker/community.svg)](https://gitter.im/Cocktail-Shaker/community?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)
![Python 3.6](https://img.shields.io/badge/python-3.6-blue.svg)
 [![DOI](https://zenodo.org/badge/170644606.svg)](https://zenodo.org/badge/latestdoi/170644606)


----

Cocktail Shaker is a **high-performance drug enumeration and expansion library**. Cocktail Shaker leverages the computational power of  **RDKit** to create and enumerate large volumes of drug compounds. 

-  File parsing of TXT, SDF, and Chemical Smiles. 
-  File writing in a variety of formats some of which include: cif, sdf, pdb, mol, mol2 and many others
-  Ability to recognize and expand libraries of compounds some of which include halogens, acyl halides, aldehydes. 
-  Ability to enumerate in 1D, and 2D structures and produce those compounds. 


Announcements
-------------

- **Release!** Version 1.0.0-beta, August 26, 2019
- **RDkit UGM 2019**: talk at September 25th at the University of Hamburg, Germany.


Using Cocktail Shaker
---------------------

Cocktail Shaker is a young library under heavy development at this time. It
targets two categories of users:

1. **Users knowing RDKit**, or willing to learn RDKit, who want to
   create fast sets of data for high throughput screening or machine learning.
2. **Open Science Scientists without any knowledge of RDKit**, who are seeking a
   a high-level wrapper to create chemical files for their software.

If you're in the first category, you can already start using RDKit.
Cocktail Shaker offers a Pythonic, easy-to-use library and you can start channeling molecules in the expansion library.
Instead of validating the sanity of the data, Cocktail Shaker takes care of that for you.
With each molecule being generated it will head into a 1D, and or 2D validation check (3D not supported yet). 

If you're in the second category, we're starting to build experimental
high-level python code to take care a lot of the underpinnings of RDKit.

Installation (TBD)
------------------

Cocktail Shaker runs on Python 3.3+ and depends on RDKit. 


Cocktail Shaker can be installed either via `pip`:

```
pip install
```

or within the `Anaconda <https://www.anaconda.com/download/>`_ Python
distribution. Anaconda provides a convenient package management system.
Installing VisPy can then easily be achieved by adding `conda-forge` to the
channels with:

```
conda config --add channels conda-forge
```

Once the `conda-forge` channel has been enabled, `vispy` can be installed with:

```
conda install 
```

Development Installation
------------------------

As Cocktail Shaker is under heavy development at this time, we highly recommend
developers to use the development version on Github (master branch). You need
to clone the repository and install VisPy with
``python setup.py install``.

As a one-liner, assuming `git` is installed::

    git clone https://github.com/Sulstice/Cocktail-Shaker.git

This will automatically install the latest version of Cocktail Shaker.

Structure of Cocktail Shaker
----------------------------

Currently, the main subpackages are:

-  **root**: Contains a lot of the high level functionality; Request Handling, File Parsing/Writing, Enumeration and Expansion
-  **docs**: An access point for the readthedocs implementation. 
-  **datasources**: This is where the system stores it's data on predfined functional groups and/or shapes (coming soon). 
-  **tests**: Tests that are for the file handling, requests, and testing molecule pattern recognition

The API of all public interfaces are subject to change in the future,
although **datasources** are *relatively* stable at this point.


Genesis
-------

Cocktail Shaker began when one developer/scientist wanted an open source drug library. 
`Suliman sharif <http://sulstice.github.io/>`

Now Cocktail Shaker looks to build on the expertise of these developers/scientists and the
broader open-science community to build an effective drug library. 

----

External links
--------------

-  `Documentation <http://cocktail-shaker.readthedocs.org>`__
