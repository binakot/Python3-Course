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
