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

## Images

I use different images for all my projects, by doing that I can also specify all the requirements needed for running them.

## Port forwarding

The server uses port `8443`.

## Environment variables

I set `DEFAULT_WORKSPACE` to `/workspace`, otherwise the default workspace would be under the config folder.

Other variables that you should set:

- `PGID`
- `PUID`
- `PASSWORD`
- `SUDO_PASSWORD`

## Binds

You should bind these:

- `/config`
- `/workspace`

To something on the host.

# Dockerfiles and extensions that I use

## C++

See the folder `c++`.

## Python

See the folder `python`.
