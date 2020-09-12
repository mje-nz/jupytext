![](https://raw.githubusercontent.com/mwouts/jupytext/master/docs/logo.png)

![CI (pip)](https://github.com/mwouts/jupytext/workflows/CI%20(pip)/badge.svg)
![CI (conda)](https://github.com/mwouts/jupytext/workflows/CI%20(conda)/badge.svg)
[![Documentation Status](https://readthedocs.org/projects/jupytext/badge/?version=latest)](https://jupytext.readthedocs.io/en/latest/?badge=latest)
[![codecov.io](https://codecov.io/github/mwouts/jupytext/coverage.svg?branch=master)](https://codecov.io/gh/mwouts/jupytext/branch/master)
[![Language grade: Python](https://img.shields.io/lgtm/grade/python/g/mwouts/jupytext.svg)](https://lgtm.com/projects/g/mwouts/jupytext/context:python)
[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
[![GitHub language count](https://img.shields.io/github/languages/count/mwouts/jupytext)](docs/languages.md)
[![Conda Version](https://img.shields.io/conda/vn/conda-forge/jupytext.svg)](https://anaconda.org/conda-forge/jupytext)
[![Pypi](https://img.shields.io/pypi/v/jupytext.svg)](https://pypi.python.org/pypi/jupytext)
[![pyversions](https://img.shields.io/pypi/pyversions/jupytext.svg)](https://pypi.python.org/pypi/jupytext)

Have you always wished Jupyter notebooks were plain text documents? Wished you could edit them in your favorite IDE? And get clear and meaningful diffs when doing version control? Then... Jupytext may well be the tool you're looking for!

Jupytext can save Jupyter notebooks as Markdown files or as scripts in [many languages](docs/languages.md).

With Jupytext, text files (`.md` and `.py`, and many others) become notebooks. You can open, edit and run them in Jupyter (right click, and _open with notebook_). You can also edit the text notebooks in any text editor, and reload them in Jupyter to get the latest changes there.

Jupytext also offers [paired notebooks](docs/paired-notebooks.md), a mode in which notebooks are saved to both a classical `.ipynb` file and to an *editable* text file. In this mode you get all the convenience of the `.ipynb` file (e.g. outputs are persisted on disk), with all the advantages of the text notebooks (version control, easy editing, etc).

Jupytext implements many text [formats](docs/formats.md) for Jupyter Notebooks. If your notebook is mostly made of code, you will probably prefer to save it as a script:
-  Use the [percent format](docs/formats.md#the-percent-format), a format with explicit cell delimiters (`# %%`), supported by many IDE (Spyder, Hydrogen, VS Code, PyCharm and PTVS).
-  Or use the [light format](docs/formats.md#the-light-format), if you prefer to see fewer cell markers.

If your notebook contains more text than code, if you are writing a documentation or a book, you probably want to save your notebook as a Markdown document.
- Use the [Jupytext Markdown format](docs/formats.md#jupytext-markdown) if you wish to render your notebook as a `.md` file (without its outputs) on GitHub.
- Use the [MyST Markdown format](docs/formats.md#myst-markdown), a markdown flavor that “implements the best parts of reStructuredText”, if you wish to render your notebooks using Sphinx or [Jupyter Book](https://jupyterbook.org).
- Finally, if you want to open your Jupyter Notebooks in RStudio, use the [R Markdown format](formats.md#r-markdown).

Jupytext is easy to [install](docs/install.md). Run either
```bash
pip install jupytext
```
or
```bash
conda install jupytext -c conda-forge
```
Restart your Jupyter server... and enjoy text notebooks (right-click, _open with notebook_) and paired notebooks (_pair notebook with..._ in the [Jupyter Commands](docs/install.md#jupytext-commands-in-jupyterlab))!

If you're new to Jupytext, you may want to start with the [FAQ](docs/faq.md) or the [Tutorials](docs/tutorials.md).
