## Quake 2 Docker Instructions

This container is built off of the inanimate/quake2 container.

To run, clone this repo and run the following on your Docker host:
```
docker run -d \
    -v ./pak0.pak:/usr/share/games/quake2/baseq2/pak0.pak \
    -v ./server.cfg:/usr/share/games/quake2/baseq2/server.cfg \
    inanimate/quake2 +fraglimit 50
```
