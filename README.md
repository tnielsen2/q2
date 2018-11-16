## Quake 2 Docker Instructions

This container is built off of the inanimate/quake2 container.

To run, clone this repo int your /opt/q2 directory:

```
git clone https://github.com/tnielsen2/q2.git /opt/q2
```

and run the following on your Docker host:
```
docker run -d \
    -v /opt/q2/pak0.pak:/usr/share/games/quake2/baseq2/pak0.pak \
    -v /opt/q2/server.cfg:/usr/share/games/quake2/baseq2/server.cfg \
    inanimate/quake2 +fraglimit 50
```
