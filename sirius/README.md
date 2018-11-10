# sirius

Little Printer Server Dockerfile.

Based on [@genmon](https://github.com/genmon)'s [sirius](https://github.com/genmon/sirius) Little Printer Server and my DIY installation guide: [Installing Sirius on Mac/Linux](https://gist.github.com/hako/f8944cfa7b8fb8115f6d).

Docker Repository: [hakobyte/sirius](https://hub.docker.com/r/hakobyte/sirius/)

### usage

To have sirius up and running on your machine, run:

`docker run -t -p 5000:5000 hakobyte/sirius /usr/bin/honcho start`

This command will pull the `hakobyte/sirius` image from Docker Hub and will run the server on port 5000.

[http://localhost:5000](http://localhost:5000)

### info

This dockerfile uses the alpine image because alpine images are tiny. 

This image is 128 MB compressed and ~296.1 MB uncompressed.
