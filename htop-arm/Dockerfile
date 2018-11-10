#
# Dockerfile for htop on ARM devices.
# (c) hako
#

FROM easypi/alpine-arm
MAINTAINER Wesley Hill <wesley@hakobaito.co.uk>
RUN apk add --update htop && rm -rf /var/cache/apk/*
ENTRYPOINT ["htop"]
