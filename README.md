# Remoll Singularity

## Building this image

```
singularity create remoll.img
sudo singularity bootstrap remoll.img Singularity
```

## Running Remoll and getting the output

```
singularity pull shub://narrative/remoll-singularity
singularity run --bind `pwd`:/jlab/2.1/Linux_CentOS7.3.1611-x86_64-gcc4.8.5/remoll/rootfiles/ \
    narrative-remoll-singularity-master.simg \
    macros/tests/test_moller.mac
```
