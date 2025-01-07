# Basic NLTK examples

This simple project holds multiple examples for using 
[Natural Language Toolkit](https://www.nltk.org/index.html).

NLTK is a leading platform for building Python programs to work with human language data. 

Before starting please read the following on how to install and use [NLTK data](https://www.nltk.org/data.html).

If we decide to use all the modules at once we would have to download a great amount of data. 
Thus we could only include modules we need in the Dockerfile.

To use a data set, just add or update the list of data sets in the Dockerfile with the data set id - listed [here](https://www.nltk.org/nltk_data/).

By defaule we only include `vader_lexicon` in the Dockerfile.

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
pipenv run python vader.py
```
