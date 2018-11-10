# htop-arm

htop for ARM devices. (Raspberry Pi, NAS Synology, etc.)

This image is useful if you have a NAS, Raspberry Pi or any ARM boards with docker on it.

Docker Repository: [hakobyte/htop-arm](https://hub.docker.com/r/hakobyte/htop-arm/)

### usage

#### run htop and see host processes

`docker run -it --rm --pid=host hakobyte/htop-arm`

### info

This dockerfile uses the alpine image because alpine images are tiny.

This image is 3 MB compressed and ~8.31 MB uncompressed.
