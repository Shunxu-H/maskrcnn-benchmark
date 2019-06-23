# Docker Manual

This is the documentation of the command we use to build a nvidia-docker image 


### Prerequisites
* docker
* nvidia-docker


### Commands 

To build the image 

```
nvidia-docker build -t maskrcnn docker/
```

To start a docker image with the binded mount

```
docker run -it maskrcnn --name maskrcnn-shareddir --mount type=bind,source=/home/${USER}/maskrcnn-virtualenv,target=/dev-env bash
```

## Versioning

We use [SemVer](http://semver.org/) for versioning. For the versions available, see the [tags on this repository](https://github.com/your/project/tags). 

## Authors

* **Facebook** - *Initial work* - [Facebook Research](https://github.com/facebookresearch/maskrcnn-benchmark)



## Acknowledgments

* Hat tip to anyone whose code was used
* Inspiration
* etc
