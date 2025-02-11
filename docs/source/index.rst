Sphinx Dokumentation documentation
==================================

Add your content using ``reStructuredText`` syntax. See the
`reStructuredText <https://www.sphinx-doc.org/en/master/usage/restructuredtext/index.html>`_
documentation for details.


.. toctree::
   :maxdepth: 2
   :caption: Contents:
Sphinx
========

Windows Installation
---------------------

# in virtual environment:

``python -m venv myenv``

``myenv\Scripts\activate``

# Installation

``pip install -U sphinx``

- install Theme

``pip install sphinx-rtd-theme``

--------------------------------------------------------------------

``mkdir docs ``

``cd docs``

``sphinx-quickstart``

yes and follow the questions

Configuration
------------------

# in docs/source/conf.py

``
import os
import sys
sys.path.insert(0, os.path.abspath('..'))

``

- ``extensions = ["sphinx.ext.autodoc", "sphinx.ext.viewcode", "sphinx.ext.napoleon"]``

- ``html_theme = 'sphinx_rtd_theme'``



- ``sphinx-build -b html source build``


- then you can use ``make html``

- edit and add rst Files!

