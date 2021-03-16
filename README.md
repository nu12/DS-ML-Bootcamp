
# Python for Data Science and Machine Learning Bootcamp

Notes from [Python for Data Science and Machine Learning Bootcamp](https://www.udemy.com/course/python-for-data-science-and-machine-learning-bootcamp/).

# Setup

## Docker

The Docker image contains everything that is needed to run the projects. Notebook is available on port 8888. Run:

```shell
$ docker-compose up
```

To access Tensorboard run `$ docker exec ds-ml-bootcamp_notebooks_1 tensorboard --logdir /notebooks/logs/fit --host 0.0.0.0 --port 6006`. Access Tensorboard on port 6006. Change `--logdir` accordingly.

## Windows setup

Install Anaconda. Tensorflow and Spark won't be available.

## Linux setup

```shell
$ python3 -m virtualenv env -p python3.8 --always-copy
$ source env/bin/activate
(env)$ pip install numpy pandas nltk matplotlib seaborn sklearn jupyter tensorflow
(env)$ jupyter notebook
```

Follow additional steps to include Spark in the Linux setup.

### PySpark

Follow this [Setup guide](https://medium.com/@josemarcialportilla/getting-spark-python-and-jupyter-notebook-running-on-amazon-ec2-dec599e1c297) to run Spark locally or on a EC2 instance. Note: After setp 7 run `sudo chmod 777 mycert.pem` to avoid permission errors.
