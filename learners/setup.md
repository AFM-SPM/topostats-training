---
title: Setup
---

This course teaches you the basics of using [TopoStats][topostats] to process Atomic Force Microscopy images. TopoStats
is software written in the [Python][python] programming language so you will need this installed on your system. Most
GNU/Linux and OSX operating systems already have Python installed however in order to make a reproducible environment
available we will guide you through how to use [Conda][conda] environments to setup and install an isolated environment
for installing TopoStats and its dependencies.

Because of the vast heterogeneity in AFM images we have created a sample data set for you to work through this tutorial
with. If time permits at the end of the class you can try processing your own images and instructors may be able to help
with any problems that you encounter.

## Data Sets

The [DNA](data/Minicircles.zip) dataset consists of Bruker AFM files of DNA minicircles (339bp) imaged on a mica surface. The two subfolders contained within show samples of relaxed (∆Lk=0) DNA minicircles, and undertwisted (∆Lk=-3) DNA minicircles. The aim of this dataset analysis is to characterise the geometric differences when the DNA helix is underwound (or negitively supercoiled).

The [Protein](data/Protein.zip) dataset consists of Bruker AFM files of the autophagy receptor protein NDP52 imaged on a mica surface. This protein is represented by a SKICH domain connected through a coiled-coil to a Zinc-finger domain. The analysis of this dataset is to help characterise this flexible protein in comparison to it's crystal structure.

Download the above datasets and and unzip them to your Desktop.

## Software Setup

::::::::::::::::::::::::::::::::::::::: discussion

### Conda

[Conda][conda] is an open-source, cross-platform, language-agnostic package manager and environment
management system for the popular programming and data science languages [Python][python] and [R][r]. For the purposes
of this class we will only be using the support for Python.

We ask that you install Conda on your laptops prior to the class so we can maximise the time available for covering the
course material. You do _not_ need to worry about creating any Conda environments before the class starts, we cover that
as part of the material.

The official [installation instructions](https://docs.conda.io/projects/conda/en/stable/user-guide/install/index.html)
are comprehensive and detailed and should get you setup.

If you find you are having problems installing the software please contact [the
instructors](mailto:topostats@sheffield.ac.uk) for assistance.

:::::::::::::::::::::::::::::::::::::::::::::::::::

:::::::::::::::: solution

### Windows

[Installing Conda on Windows](https://docs.conda.io/projects/conda/en/stable/user-guide/install/windows.html)

:::::::::::::::::::::::::

:::::::::::::::: solution

### MacOS

[Installing Conda on macOS](https://docs.conda.io/projects/conda/en/stable/user-guide/install/macos.html)

:::::::::::::::::::::::::


:::::::::::::::: solution

### Linux

[Installing Conda on Linux](https://docs.conda.io/projects/conda/en/stable/user-guide/install/linux.html)

:::::::::::::::::::::::::

[conda]: https://docs.conda.io/en/latest/
[python]: https://www.python.org
[r]: https://www.r-project.org/
[topostats]: https://afm-spm.github.io/TopoStats
