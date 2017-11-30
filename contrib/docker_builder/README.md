# Dockerfile for building CannabisCoin binaries.

Now, you can build your own CannabisCoin files on all systems with docker and do it easy without installing depends on your system.

## How:

### Build docker image

```
sudo docker build .
```

### Run docker container

Builder will return HASH of image
Example:
Successfully built 9bbff825d50f

```
sudo docker run -it -v ~/path/to/CannabisCoin/folder:/CannabisCoin 9bbff825d50f
```

If your system uses SELINUX you may use --privileged=true key

```
sudo docker run --privileged=true -it -v ~/development/CannabisCoin:/CannabisCoin 9bbff825d50f
```

See CannabisCoin-qt file in used CannabisCoin folder and CannabisCoind file in src subfolder.