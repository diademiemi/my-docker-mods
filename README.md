# Java 16 - Docker mod for code-server

This mod adds AdoptOpenJDK Java 16 to code-server, to be installed/updated during container start.

In code-server docker arguments, set an environment variable `DOCKER_MODS=ghcr.io/diademiemi/docker-mods:code-server-java16`

If adding multiple mods, enter them in an array separated by `|`, such as `DOCKER_MODS=ghcr.io/diademiemi/docker-mods:code-server-java16|linuxserver/mods:openssh-server-mod2`
