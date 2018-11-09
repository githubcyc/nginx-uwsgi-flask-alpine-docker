
## Get Started

* run

```
cd python3 
docker-compose up
docker-compose down
```

* python3-science

```bash
docker build -t python3-science:1.0 .
docker run -ti python3-science sh
pip list
```

A lightweight **Alpine Linux** Docker container image for **Flask** application served by **uWSGI** and **NGINX**, managed by **Supervisord**. Read all about it in [this blog post](https://netdevops.me/2017/flask-application-in-a-production-ready-container/).

## Refer

* [uwsgi-nginx-flask-docker: Docker image with uWSGI and Nginx for Flask applications in Python running in a single container. Optionally with Alpine Linux.](https://github.com/tiangolo/uwsgi-nginx-flask-docker)
* [jfloff/alpine-python: A small, more complete, Python Docker image based on Alpine Linux.](https://github.com/jfloff/alpine-python)
* [frol/docker-alpine-python-machinelearning: Small Docker image with Python Machine Learning tools (~180MB) https://hub.docker.com/r/frolvlad/alpine-python-machinelearning/](https://github.com/frol/docker-alpine-python-machinelearning)