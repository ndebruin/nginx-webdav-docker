# nginx-webdav-docker

An Alpine Docker container that runs nginx as a WebDAV server.


# Usage:

Usage is very simple, as there is very little this container actually does. No TLS, no authentication. All of that should be handled on a Reverse Proxy.

```
docker run --name nginx-webdav -p 80:80 -v /path/to/content:/srv/:rw -d ghcr.io/ndebruin/nginx-webdav-docker:latest
```

You can change the port number.

You need to change the host path, that is where the files you want served go.
