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

