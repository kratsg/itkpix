# `itkpix`: metapackage for ITk Pixels

[![image](https://img.shields.io/pypi/v/itkpix.svg)](https://pypi.python.org/pypi/itkpix)

[![image](https://img.shields.io/conda/vn/conda-forge/itkpix.svg)](https://github.com/conda-forge/itkpix-feedstock)

[![image](https://zenodo.org/badge/DOI/10.5281/zenodo.1043949.svg)](https://doi.org/10.5281/zenodo.1043949)

[![image](https://github.com/kratsg/itkpix/workflows/CI/badge.svg)](https://github.com/kratsg/itkpix/actions?query=workflow%3ACI+branch%3Amain)

[![image](https://codecov.io/gh/kratsg/itkpix/graph/badge.svg?branch=main)](https://codecov.io/gh/kratsg/itkpix?branch=main)

## Project info

The [ITk project](https://itk.docs.cern.ch/) is an ATLAS-driven
and ATLAS-oriented project with the aim of providing python package tooling for upgrade work in ITk Pixels.

## itkpix package

`itkpix` is a metapackage for the ITk Pixels project.

### Installation

You can install this metapackage from PyPI with \`pip\`:

``` bash
python -m pip install itkpix
```

or you can use Conda through conda-forge:

``` bash
conda install -c conda-forge itkpix
```

All the normal best-practices for Python apply; you should be in a
virtual environment, etc.

### Package version and dependencies

Please check the `setup.cfg` and `requirements.txt` files for the list
of Python versions supported and the list of ITk Pixels project packages
and dependencies included, respectively.

For any installed `itkpix` the following displays the actual
versions of all ITk Pixels dependent packages installed, for example:

``` python
>>> import itkpix
>>> itkpix.show_versions()

System:
    python: 3.9.12 (main, Apr  4 2022, 05:22:27) [MSC v.1916 64 bit (AMD64)]
executable: C:\home\sw\anaconda3\python.exe
   machine: Windows-10-10.0.19044-SP0

Python dependencies:
       pip: 21.2.4
setuptools: 61.2.0
     numpy: 1.21.5
     scipy: 1.7.3
    pandas: 1.4.2
matplotlib: 3.5.1

SITk Pixels package version and dependencies:
        awkward: 1.8.0
boost_histogram: 1.3.1
  decaylanguage: 0.14.2
       hepstats: 0.5.0
       hepunits: 2.2.1
           hist: 2.6.1
     histoprint: 2.4.0
        iminuit: 2.16.0
         mplhep: 0.3.26
       particle: 0.20.1
          pylhe: 0.4.0
       resample: 1.5.1
          skhep: 4.1.0
         uproot: 4.3.5
         vector: 0.8.5
```

**Note on the versioning system:**

-   A version `itkpix x.y` is compatible with the releases of all
    package dependents versions `a.b.c` for all `c`.
-   Major version updates are prepared every time (at least) a \"package
    component\" does the same.
-   Minor version updates are the typical updates, when (at least) a
    package goes from version `a.b` to `a.(b+1)`.
-   Patch version updates are only done if there is some reason on the
    side of the metapackage itself.
