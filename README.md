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

* Python language: [https://www.python.org](https://www.python.org).

* Python Package Index (PyPI): [https://pypi.org](https://pypi.org).

* Package installer for Python (PIP): [https://pypi.org/project/pip](https://pypi.org/project/pip).

* Python Virtual Environment (VENV): [https://virtualenv.pypa.io/en/latest](https://virtualenv.pypa.io/en/latest).

### Development

* Python type hints: [https://docs.python.org/3/library/typing.html](https://docs.python.org/3/library/typing.html).

* Python data classes: [https://docs.python.org/3/library/dataclasses.html](https://docs.python.org/3/library/dataclasses.html).

* Functions creating iterators for efficient looping: [https://docs.python.org/3/library/itertools.html](https://docs.python.org/3/library/itertools.html).

### Tests & Lints

* Unit testing framework: [https://docs.python.org/3/library/unittest.html](https://docs.python.org/3/library/unittest.html).

* Test interactive Python examples: [https://docs.python.org/3/library/doctest.html](https://docs.python.org/3/library/doctest.html).

* Python static code analysis tool: [https://www.pylint.org](https://www.pylint.org).

* Python tool that glues together pep8, pyflakes, mccabe, and third-party plugins: [https://gitlab.com/pycqa/flake8](https://gitlab.com/pycqa/flake8).

### Dependencies

* Requests is an elegant and simple HTTP library for Python: [https://requests.readthedocs.io/en/master](https://requests.readthedocs.io/en/master).

* Flask is a micro web framework written in Python: [https://flask.palletsprojects.com](https://flask.palletsprojects.com).

---

## Computer & Data Science

### Common

* Greedy algorithms: [https://en.wikipedia.org/wiki/Greedy_algorithm](https://en.wikipedia.org/wiki/Greedy_algorithm).

* Dynamic programming: [https://en.wikipedia.org/wiki/Dynamic_programming](https://en.wikipedia.org/wiki/Dynamic_programming).

### Classification & Regression

* K-nearest neighbors: [https://en.wikipedia.org/wiki/K-nearest_neighbors_algorithm](https://en.wikipedia.org/wiki/K-nearest_neighbors_algorithm).

* Naive Bayes: [https://en.wikipedia.org/wiki/Naive_Bayes_classifier](https://en.wikipedia.org/wiki/Naive_Bayes_classifier).

* Decision tree: [https://en.wikipedia.org/wiki/Decision_tree](https://en.wikipedia.org/wiki/Decision_tree).

### Python

#### Libraries

* Numerical computing with Python: [https://numpy.org](https://numpy.org).

#### Anaconda

* Open source projects provided by Anaconda: [https://www.anaconda.com/open-source](https://www.anaconda.com/open-source).

* Anaconda blog: [https://www.anaconda.com/blog](https://www.anaconda.com/blog).

#### Jupiter

* Jupiter Widgets gallery: [https://jupyter.org/widgets](https://jupyter.org/widgets).

* Jupyter Notebooks gallery: [https://nbviewer.jupyter.org](https://nbviewer.jupyter.org).
