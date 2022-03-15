# nginx-fancyindex-docker

An Alpine Docker container that runs nginx along with the fancyindex mod.


# Usage:

Usage is very simple, as there is very little this container actually does.

```
docker run --name nginx-fancyindex -p 80:80 -v /path/to/content:/srv/:ro -d registry.gitlab.draigon.org/ndebruin/nginx-fancyindex-docker:latest
```

You can change the port number.

You need to change the host path, that is where the files you want served go.
