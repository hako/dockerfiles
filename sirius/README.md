# sirius

A Little Printer Server Dockerfile.

Based on [@genmon's](https://github.com/genmon) sirius little printer server.

### [genmon/sirius](https://github.com/genmon/sirius)

and my DIY installation guide:

### [Installing Sirius on Mac/Linux](https://gist.github.com/hako/f8944cfa7b8fb8115f6d)

To have sirius up and running on your machine, run:

`docker run -t -p 5000:5000 hakobyte/sirius /usr/bin/honcho start`

This command will pull the `hakobyte/sirius` image from Docker Hub and will run the server on port 5000.

[http://localhost:5000](http://localhost:5000)

This dockerfile uses the alpine image because alpine images are tiny. 

This image is (296.1 MB approx)