# graphical
Base docker image for graphical apps

To start graphical apps in a container mount X11 socket and set DISPLAY variable:

```
docker run -d --rm
	-v /tmp/.X11-unix:/tmp/.X11-unix \
	-e DISPLAY=unix$DISPLAY \
	graphical:latest \
	/grahical/app
```
