# Introduction
The material in this repository shows how to create slides using Jupyter.


# Running Jupyter
If you are at least somewhat familiar with Docker, the easiest way to run Jupyter is by using the [Jupyter Docker Stacks](https://jupyter-docker-stacks.readthedocs.io/en/latest/), a set of Docker images containing Jupyter applications and interactive computing tools and maintained by the Jupyter team.

As an example, to run a `scipy-notebook`, a Jupyter Docker Stacks image that includes numerous packages from the Python's scientific ecosystem, you can simply issue:

```shell
$ docker run -p 8888:8888 jupyter/scipy-notebook
```

The output of the above command will look something like this:

```shell
Unable to find image 'jupyter/scipy-notebook:latest' locally
latest: Pulling from jupyter/scipy-notebook
692c352adcf2: Pull complete 

// <-- snip -->

Digest: sha256:a80a324d6edd498bed32211c1d5f6c1e68c09fee9a8d5c08308e34a68aa81b0a
Status: Downloaded newer image for jupyter/scipy-notebook:latest
Executing the command: jupyter notebook
[I 21:07:52.120 NotebookApp] Writing notebook server cookie secret to /home/jovyan/.local/share/jupyter/runtime/notebook_cookie_secret
[I 21:07:52.657 NotebookApp] JupyterLab extension loaded from /opt/conda/lib/python3.8/site-packages/jupyterlab
[I 21:07:52.657 NotebookApp] JupyterLab application directory is /opt/conda/share/jupyter/lab
[I 21:07:52.659 NotebookApp] Serving notebooks from local directory: /home/jovyan
[I 21:07:52.659 NotebookApp] Jupyter Notebook 6.1.3 is running at:
[I 21:07:52.659 NotebookApp] http://82616606a5ca:8888/?token=664faad07ab446765bf2e388ff90538a3c11848655290f7c
[I 21:07:52.659 NotebookApp]  or http://127.0.0.1:8888/?token=664faad07ab446765bf2e388ff90538a3c11848655290f7c
[I 21:07:52.659 NotebookApp] Use Control-C to stop this server and shut down all kernels (twice to skip confirmation).
[C 21:07:52.662 NotebookApp] 
    
    To access the notebook, open this file in a browser:
        file:///home/jovyan/.local/share/jupyter/runtime/nbserver-6-open.html
    Or copy and paste one of these URLs:
        http://82616606a5ca:8888/?token=664faad07ab446765bf2e388ff90538a3c11848655290f7c
     or http://127.0.0.1:8888/?token=664faad07ab446765bf2e388ff90538a3c11848655290f7c
[I 21:10:15.665 NotebookApp] 302 GET /?token=664faad07ab446765bf2e388ff90538a3c11848655290f7c (172.17.0.1) 1.48ms
```
To access the Jupyter notebook, you can point your web browser to `http://127.0.0.1:8888/?token=664faad07ab446765bf2e388ff90538a3c11848655290f7c` (the token on your machine will be different from mine).

# Creating the Slides

# Exporting the Slides to Static HTML or PDF
