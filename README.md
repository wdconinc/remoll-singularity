# Remoll Singularity

## Setup

### Adding NeuroDebian sources:

Follow instructions [here](http://neuro.debian.net/) to add the Singularity sources to package manager.

### Install Singularity

```
sudo apt update && apt install -y singularity-container
```

## Building this image

```
singularity create remoll.img
sudo singularity bootstrap remoll.img Singularity
```

## Running Remoll and getting the output

```
singularity run --bind `pwd`:/jlab/2.1/Linux_CentOS7.3.1611-x86_64-gcc4.8.5/remoll/rootfiles/ remoll.img macros/tests/test_moller.mac
```

