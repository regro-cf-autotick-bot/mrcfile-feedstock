<!--
# -*- mode: jinja -*-
-->

About mrcfile
=============

Home: https://github.com/ccpem/mrcfile

Package license: BSD

Feedstock license: BSD 3-Clause

Summary: MRC file I/O library

mrcfile is a Python implementation of the MRC2014 file format
(http://www.ccpem.ac.uk/mrc_format/mrc2014.php), which is used in
structural biology to store image and volume data.

It allows MRC files to be created and opened easily using a very
simple API, which exposes the file's header and data as numpy
arrays. The code runs in Python 2 and 3 and is fully unit-tested.

This library aims to allow users and developers to read and write
standard-compliant MRC files in Python as easily as possible, and
with no dependencies on any compiled libraries except numpy. You can
use it interactively to inspect files, correct headers and so on, or
in scripts and larger software packages to provide basic MRC file
I/O functions.


Current build status
====================

[![Linux](https://img.shields.io/circleci/project/github/conda-forge/mrcfile-feedstock/master.svg?label=Linux)](https://circleci.com/gh/conda-forge/mrcfile-feedstock)
[![OSX](https://img.shields.io/travis/conda-forge/mrcfile-feedstock/master.svg?label=macOS)](https://travis-ci.org/conda-forge/mrcfile-feedstock)
[![Windows](https://img.shields.io/appveyor/ci/conda-forge/mrcfile-feedstock/master.svg?label=Windows)](https://ci.appveyor.com/project/conda-forge/mrcfile-feedstock/branch/master)

Current release info
====================

| Name | Downloads | Version | Platforms |
| --- | --- | --- | --- |
| [![Conda Recipe](https://img.shields.io/badge/recipe-mrcfile-green.svg)](https://anaconda.org/conda-forge/mrcfile) | [![Conda Downloads](https://img.shields.io/conda/dn/conda-forge/mrcfile.svg)](https://anaconda.org/conda-forge/mrcfile) | [![Conda Version](https://img.shields.io/conda/vn/conda-forge/mrcfile.svg)](https://anaconda.org/conda-forge/mrcfile) | [![Conda Platforms](https://img.shields.io/conda/pn/conda-forge/mrcfile.svg)](https://anaconda.org/conda-forge/mrcfile) |

Installing mrcfile
==================

Installing `mrcfile` from the `conda-forge` channel can be achieved by adding `conda-forge` to your channels with:

```
conda config --add channels conda-forge
```

Once the `conda-forge` channel has been enabled, `mrcfile` can be installed with:

```
conda install mrcfile
```

It is possible to list all of the versions of `mrcfile` available on your platform with:

```
conda search mrcfile --channel conda-forge
```


About conda-forge
=================

[![Powered by NumFOCUS](https://img.shields.io/badge/powered%20by-NumFOCUS-orange.svg?style=flat&colorA=E1523D&colorB=007D8A)](http://numfocus.org)

conda-forge is a community-led conda channel of installable packages.
In order to provide high-quality builds, the process has been automated into the
conda-forge GitHub organization. The conda-forge organization contains one repository
for each of the installable packages. Such a repository is known as a *feedstock*.

A feedstock is made up of a conda recipe (the instructions on what and how to build
the package) and the necessary configurations for automatic building using freely
available continuous integration services. Thanks to the awesome service provided by
[CircleCI](https://circleci.com/), [AppVeyor](https://www.appveyor.com/)
and [TravisCI](https://travis-ci.org/) it is possible to build and upload installable
packages to the [conda-forge](https://anaconda.org/conda-forge)
[Anaconda-Cloud](https://anaconda.org/) channel for Linux, Windows and OSX respectively.

To manage the continuous integration and simplify feedstock maintenance
[conda-smithy](https://github.com/conda-forge/conda-smithy) has been developed.
Using the ``conda-forge.yml`` within this repository, it is possible to re-render all of
this feedstock's supporting files (e.g. the CI configuration files) with ``conda smithy rerender``.

For more information please check the [conda-forge documentation](https://conda-forge.org/docs/).

Terminology
===========

**feedstock** - the conda recipe (raw material), supporting scripts and CI configuration.

**conda-smithy** - the tool which helps orchestrate the feedstock.
                   Its primary use is in the construction of the CI ``.yml`` files
                   and simplify the management of *many* feedstocks.

**conda-forge** - the place where the feedstock and smithy live and work to
                  produce the finished article (built conda distributions)


Updating mrcfile-feedstock
==========================

If you would like to improve the mrcfile recipe or build a new
package version, please fork this repository and submit a PR. Upon submission,
your changes will be run on the appropriate platforms to give the reviewer an
opportunity to confirm that the changes result in a successful build. Once
merged, the recipe will be re-built and uploaded automatically to the
`conda-forge` channel, whereupon the built conda packages will be available for
everybody to install and use from the `conda-forge` channel.
Note that all branches in the conda-forge/mrcfile-feedstock are
immediately built and any created packages are uploaded, so PRs should be based
on branches in forks and branches in the main repository should only be used to
build distinct package versions.

In order to produce a uniquely identifiable distribution:
 * If the version of a package **is not** being increased, please add or increase
   the [``build/number``](https://conda.io/docs/user-guide/tasks/build-packages/define-metadata.html#build-number-and-string).
 * If the version of a package **is** being increased, please remember to return
   the [``build/number``](https://conda.io/docs/user-guide/tasks/build-packages/define-metadata.html#build-number-and-string)
   back to 0.

Feedstock Maintainers
=====================

* [@bkpoon](https://github.com/bkpoon/)
* [@colinpalmer](https://github.com/colinpalmer/)

