# Python3 Course

Run [Anaconda](https://docs.anaconda.com/anaconda)
with [Jupiter Notebook](https://jupyter-notebook.readthedocs.io/en/stable/notebook.html)
via `Docker` container:

```bash
$ docker pull continuumio/anaconda3

$ docker run \
  --name anaconda3-jupyter-notebook \
  -p 8888:8888 \
  -v $(pwd)/notebooks:/opt/notebooks \
  -d continuumio/anaconda3 \
  /bin/bash -c "/opt/conda/bin/conda install jupyter -y --quiet && /opt/conda/bin/jupyter notebook --notebook-dir=/opt/notebooks --ip='*' --port=8888 --no-browser --allow-root"

$ docker container logs anaconda3-jupyter-notebook
```

Now open [http://localhost:8888](http://localhost:8888) with a token from container logs.

---

# Useful links

## Python

* Python language: 
  [https://www.python.org](https://www.python.org).

* Python Package Index (PyPI):
  [https://pypi.org](https://pypi.org).

* Package Installer for Python (PIP): 
  [https://pypi.org/project/pip](https://pypi.org/project/pip).

* Python Virtual Environment (VENV): 
  [https://virtualenv.pypa.io/en/latest](https://virtualenv.pypa.io/en/latest).

### Development

* Type hints: 
  [https://docs.python.org/3/library/typing.html](https://docs.python.org/3/library/typing.html).

* Data classes:
  [https://docs.python.org/3/library/dataclasses.html](https://docs.python.org/3/library/dataclasses.html).

* Functions creating iterators for efficient looping: 
  [https://docs.python.org/3/library/itertools.html](https://docs.python.org/3/library/itertools.html).

### Tests & Lints

* Unit testing framework: 
  [https://docs.python.org/3/library/unittest.html](https://docs.python.org/3/library/unittest.html).

* Interactive documentation tests: 
  [https://docs.python.org/3/library/doctest.html](https://docs.python.org/3/library/doctest.html).

* Static code analysis tool:
  [https://www.pylint.org](https://www.pylint.org).

* Tool that glues together pep8, pyflakes, mccabe, and third-party plugins: 
  [https://gitlab.com/pycqa/flake8](https://gitlab.com/pycqa/flake8).

### Dependencies

* The elegant and simple HTTP library:
  [https://requests.readthedocs.io](https://requests.readthedocs.io).

* Micro web framework: 
  [https://flask.palletsprojects.com](https://flask.palletsprojects.com).

---

## Computer & Data Science

### Common

* Greedy algorithms: 
  [https://en.wikipedia.org/wiki/Greedy_algorithm](https://en.wikipedia.org/wiki/Greedy_algorithm).

* Dynamic programming: 
  [https://en.wikipedia.org/wiki/Dynamic_programming](https://en.wikipedia.org/wiki/Dynamic_programming).

* Machine Learning for everyone:
  [https://vas3k.com/blog/machine_learning](https://vas3k.com/blog/machine_learning).

* Machine Learning for humans:
  [https://medium.com/machine-learning-for-humans](https://medium.com/machine-learning-for-humans).

* The neural network zoo:
  [https://www.asimovinstitute.org/neural-network-zoo](https://www.asimovinstitute.org/neural-network-zoo).

### Python

#### Libraries

* Python-based ecosystem of open-source software for mathematics, science, and engineering: 
  [https://www.scipy.org](https://www.scipy.org).

* Enhanced interactive interpreter:
  [http://ipython.org](http://ipython.org).

* Multidimensional arrays and matrices computing: 
  [https://numpy.org](https://numpy.org).

* Collection of algorithms and high-level commands for manipulating and visualizing data (builds on NumPy): 
  [https://www.scipy.org/scipylib](https://www.scipy.org/scipylib).

* Data structures and tools for data analysis (builds on NumPy): 
  [https://pandas.pydata.org](https://pandas.pydata.org).

* 2D plots and graphs: 
  [https://matplotlib.org](https://matplotlib.org).

* Data visualization library (builds on matplotlib): 
  [https://seaborn.pydata.org](https://seaborn.pydata.org).

* Graphing library makes interactive, publication-quality graphs with 3D:
  [https://plotly.com/python](https://plotly.com/python).

* Interactive visualization library for modern web browsers:
  [https://docs.bokeh.org](https://docs.bokeh.org).

* Working with geospatial data (extends the datatypes used by pandas):
  [https://geopandas.readthedocs.io](https://geopandas.readthedocs.io).

* Set of algorithms for machine learning and data mining tasks (builds on NumPy and SciPy): 
  [https://scikit-learn.org](https://scikit-learn.org).

* Deep learning framework:
  [https://keras.io](https://keras.io).

* Classes and functions for the estimation of statistical models, as well as for conducting statistical tests, and statistical data exploration ((builds on NumPy & SciPy):
  [https://www.statsmodels.org](https://www.statsmodels.org).

* Symbolic mathematics: 
  [https://www.sympy.org/en/index.html](https://www.sympy.org/en/index.html).

* Flexible library for parallel computing (integrated with NumPy, pandas, and scikit-learn):
  [https://dask.org](https://dask.org).

#### Anaconda

* Open source projects provided by Anaconda: 
  [https://www.anaconda.com/open-source](https://www.anaconda.com/open-source).

* Anaconda blog: 
  [https://www.anaconda.com/blog](https://www.anaconda.com/blog).

#### Jupiter

* Jupiter Widgets gallery: 
  [https://jupyter.org/widgets](https://jupyter.org/widgets).

* Jupyter Notebooks gallery: 
  [https://nbviewer.jupyter.org](https://nbviewer.jupyter.org).

* Data science Jupyter notebooks:
  [https://github.com/donnemartin/data-science-ipython-notebooks](https://github.com/donnemartin/data-science-ipython-notebooks).

---

### Others

* Platform for machine learning:
  [https://www.tensorflow.org](https://www.tensorflow.org).
