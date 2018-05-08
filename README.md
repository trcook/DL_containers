# TF

This  repository builds a singularity image that contains a well-functioning stack for deep learning development. Installed packages include tensorflow, tensorforce, OpenAI Gym, Keras, Numpy and Pandas. Tensorflow is installed as gpu-compatible with the appropriate cuda and cudnn libraries. Beware, this container will not run tensorflow unless the underlying processor arch supports AVX2 and SSE. 


## How to install:

At bash prompt:

```{bash}
singularity pull shub://trcook/tf:latest
```

Note the `latest` tag is necessarry. Without it, you will just download the base image which does not have tensorflow installed. 

## Usage
Use as you would use any singularity image. The runscript for the image will launch a container that dumps into python 3.5.
