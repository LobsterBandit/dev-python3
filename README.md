# python 3 dev image

> python 3 development image based on [`python:3-slim`](https://hub.docker.com/_/python/)

## Includes

- `pythonista` non-root user with sudo access
  - pass ARG USERNAME to rename
  - ARG USER_UID=1000
  - ARG USER_GID=USER_UID
- ARG LOCALE=en_US.UTF-8
- shell prompt configuration with [starship.rs](https://starship.rs/)
- [JetBrains Mono](https://www.jetbrains.com/lp/mono/) Powerline font
- packages required for vs code python extension
  - black
  - pyline
  - flake8

## Run from latest Docker hub image

```bash
docker run --rm -it lobsterbandit/dev-python3:latest
```

## Build from Dockerfile

```bash
docker build -t someimagename:sometag .
```
