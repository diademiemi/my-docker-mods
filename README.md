# Custom user mod for code-server

This mod adds NVIM to code-server, obtained from latest GitHub release, to be installed/updated during container start.

In code-server docker arguments, set an environment variable `DOCKER_MODS=ghcr.io/diademiemi/docker-mods:code-server-neovim`

If adding multiple mods, enter them in an array separated by `|`, such as `DOCKER_MODS=ghcr.io/diademiemi/docker-mods:code-server-neovim|linuxserver/mods:openssh-server-mod2`
