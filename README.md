# dind
docker in docker based on centos

Thinks to [jpetazzo/dind](https://github.com/jpetazzo/dind), I change a little bit


### Run the container with bash default

```
docker run -it --rm --name dind --privileged -v /var/lib/docker/:/var/lib/docker/   duffqiu/dind
```

- note: must use the `--privileged` parameter
- note: if you want to share the image with the docker host, you must mount the host volume `/var/lib/docker/` to the container's volume in the same path.
- note: if you want to see the docker's log in host, you can mount a local log file to `/var/log/docker.log`
 
