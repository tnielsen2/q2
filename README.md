## Quake 2 Docker Instructions

This container is built off of the drags/docker-quake2 github repo.

To run, clone this repo int your /opt/q2 directory:

```
git clone https://github.com/tnielsen2/q2.git /opt/q2
```

## Rocket Arena

Build the container
```
docker build /opt/q2/Dockerfile --tag quake2
```

Run the container:
```
docker run -d -p 27910:27910/udp
```
## Rail Arena
