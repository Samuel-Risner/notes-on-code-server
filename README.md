# notes-on-code-server

Things that I found useful.

# Info

I used the [LinuxServer.io Docker image](https://hub.docker.com/r/linuxserver/code-server): `linuxserver/code-server:4.16.1`

# More reading

You can find the documentation from Linuxserver.io under:
- https://hub.docker.com/r/linuxserver/code-server
- https://docs.linuxserver.io/images/docker-code-server

The original Repo and documentation are also quite useful:
- https://github.com/coder/code-server
- https://coder.com/docs/code-server/latest

# Setting up the container

## Image

I use different images for all my projects, by doing that I can also specify all the requirements needed for running them.

## Port forwarding

The server uses port `8443`.

## Environment variables

I set `DEFAULT_WORKSPACE` to `/workspace`, otherwise the default workspace would be under the config folder. By doing that I can easily swap out containers with different images.

Other variables that you should set:

- `PGID`
- `PUID`
- `PASSWORD`
- `SUDO_PASSWORD`

## Volumes

I set up two volumes, the first one contains all the configuration and second one contains all my code.
By having an extra container for my code I can switch out the different projects that I'm working on.
But you can do whatever you like sine changing the working directory is really easy.

Container name | Mount path
---|---
config | `/config`
some-project | `/workspace`

# Images that I use

## C++

See the folder `c++`.