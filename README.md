# Custom user mod for code-server

This mod adds a way to set a custom username and home directory to code-server, to be installed/updated during container start.

In code-server docker arguments, set an environment variable `DOCKER_MODS=ghcr.io/diademiemi/docker-mods:code-server-custom-user`

If adding multiple mods, enter them in an array separated by `|`, such as `DOCKER_MODS=ghcr.io/diademiemi/docker-mods:code-server-custom-user|linuxserver/mods:openssh-server-mod2`

Define the following environment variables in the container startup.

`USERNAME`: The username to use in the container. Must be lower case and otherwise valid Linux login name. Defaults to `abc`  
`HOME`: The home directory to use in the container. Must be a valid directory in the container. Defaults to `/config`  
`SHELL`: Path to the default shell of this user. Must be a valid shell executable in the cointainer. Defaults to `/bin/bash`  
