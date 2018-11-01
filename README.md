docker-prospector
========================
![Docker Build Status](https://img.shields.io/docker/build/fabiankoehler/prospector.svg) ![MicroBadger Size](https://img.shields.io/microbadger/image-size/fedora/apache.svg) ![MicroBadger Size](https://img.shields.io/microbadger/image-size/fedora/apache.svg)

Run python linters using [prospector](https://github.com/PyCQA/prospector) in a Docker container.
The usage of this container is similar to the one of [coala](https://coala.io/#/home?lang=Python), it is as easy as running
```
docker run -v $(pwd):/app --workdir=/app fabiankoehler/prospector
```
from your project directory.
You can pass append any of the usual prospector command line arguments, e.g.
```
docker run -v $(pwd):/app --workdir=/app fabiankoehler/prospector --help
```
The simplest way to configure prospector is to create a `.prospector.yaml` file in your project directory. Please also check out the [prospector documentation](http://prospector.readthedocs.io/).
