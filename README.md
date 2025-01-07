# Basic NLTK examples

This simple project holds multiple examples for using 
[Natural Language Toolkit](https://www.nltk.org/index.html).

NLTK is a leading platform for building Python programs to work with human language data. 

# Running with Docker

Only required prerequisite - a working installation of Docker.

To start the project run:

```bash
docker-compose up
```

Once up you should just see logs from the different containers that just started.
In another termminal execute into the running container:

```bash
docker exec -it  nltk-examples-python_app-1 bash
```

You could access the containers from the Docker Desktop UI as well. 

Once in the container you can run different NLTK examples:

```bash
pipenv run python nltk.py
```
