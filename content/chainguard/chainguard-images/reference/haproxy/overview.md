---
title: "Image Overview: haproxy"
type: "article"
description: "Overview: haproxy Chainguard Images"
date: 2022-11-01T11:07:52+02:00
lastmod: 2022-11-01T11:07:52+02:00
draft: false
images: []
menu:
  docs:
    parent: "images-reference"
weight: 600
toc: true
---

`experimental` [cgr.dev/chainguard/haproxy](cgr.dev/chainguard/haproxy)
| Tags     | Aliases                 |
|----------|-------------------------|
| `latest` | 2, 2.6, 2.6.7, 2.6.7-r2 |









A minimal haproxy base image rebuilt every night from source.

## Get It!

The image is available on `cgr.dev`:

```
docker pull cgr.dev/chainguard/haproxy:latest
```

## Usage

Similar to the `docker-library/haproxy` image, this image does not come with any default configuration.

Please refer to [upstream's excellent (and comprehensive) documentation](https://docs.haproxy.org/) on the subject of configuring HAProxy for your needs.

Let say you have a `haproxy.cfg` config file is current working directory. To test that configuration file, you can run the following command

```
docker run -it --rm -v "$(pwd):/etc/haproxy" --name haproxy-syntax-check cgr.dev/chainguard/haproxy haproxy -c -f /etc/haproxy/haproxy.cfg
```

In order for the container to work, you need to mount your custom `haproxy.cfg` file in the container. The following example runs HAProxy with a custom configuration file:

```
docker run -it --rm -v "$(pwd):/etc/haproxy" cgr.dev/chainguard/haproxy haproxy -f /etc/haproxy/haproxy.cfg
```