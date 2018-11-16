## Quake 2 Docker Instructions

This container is built off of the drags/docker-quake2 github repo.

To run, clone this repo int your /opt/q2 directory:

```
git clone https://github.com/tnielsen2/q2.git /opt/q2
```

Build the container
```
docker build /opt/q2/Dockerfile --tag quake2
```

Run the container:
```
docker run -d -p 27910:27910/udp quake2/server1
```






and run the following on your Docker host:
```
docker run -d \
    --name quake2 \
    -v /opt/q2/pak0.pak:/usr/share/games/quake2/baseq2/pak0.pak \
    -v /opt/q2/server.cfg:/usr/share/games/quake2/baseq2/server.cfg \
    inanimate/quake2 +fraglimit 50
```
