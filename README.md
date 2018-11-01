docker-prospector
========================

Run python linters using [prospector](https://github.com/PyCQA/prospector) in a Docker container.
The usage of this container is similar to the one of [coala](https://coala.io/#/home?lang=Python), it is as easy as running
```
docker run -v $(pwd):/app --workdir=/app prospector
```
from your project directory.
You can pass append any of the usual prospector command line arguments, e.g.
```
docker run -v $(pwd):/app --workdir=/app prospector --help
```
The simplest way to configure prospector is to create a `.prospector.yaml` file in your project directory. Please also check out the [prospector documentation](http://prospector.readthedocs.io/).
