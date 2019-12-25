## Build images for production

```bash
$ docker build -t twci/multi-client ./client
$ docker build -t twci/multi-worker ./worker
```

## Push images to docker hub

```bash
# Log in to docker hub
$ docker login

$ docker push twci/multi-client
```
