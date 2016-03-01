# debian-arm-xc

A Docker image of an x86 Debian Jessie machine that has the cross compilation tools for armhf installed.

## Usage

Build the container in the usual manner:

```
cd debian-arm-xc/debian-arm-xc
docker build . -t mytag/debian-xc
```

And, usually, build things by mounting your source directory:

```
cd myproject
docker run -t -i -v $PWD:/build mytag/debian-xc
./configure   # in the docker bash
make          # in the docker bash
```
