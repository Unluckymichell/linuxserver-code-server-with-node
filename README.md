# VS Code in the browser, with NodeJS pre-installed

This is an extended version of [linuxserver/code-server](https://hub.docker.com/r/linuxserver/code-server). It allows you to run VS Code on any machine anywhere and access it in the browser.

This project adds the following features/tools:

- `n`, the NodeJS version manager
- two versions of NodeJS: the current LTS version and the current stable version. You can switch between them using the `n` command inside the docker container. For example: `n lts`, or `n latest`. You can also install other Node versions, for example: `n 12`.
- `npm`, the NodeJS package manager
- `yarn`, an alternative NodeJS package manager
- `pnpm`, another alternative NodeJS package manager
- configures Git to cache your password for 15 minutes, so you don't have to enter it everytime

# Docker image

The docker image is [available in the github Package registry](https://github.com/Unluckymichell/linuxserver-code-server-with-node/pkgs/container/linuxserver-code-server-with-node) as `ghcr.io/unluckymichell/linuxserver-code-server-with-node:latest`.

It is automatically rebuilt every week (on Monday) with the latest version of the `linuxserver/code-server` image.

# Example usage

This image can be used in-place instead of the original [linuxserver](https://hub.docker.com/r/linuxserver/code-server) image.

