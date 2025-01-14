# Installation

## Oxen CLI

The Oxen client mirrors the git command line interface can be installed via [homebrew](https://brew.sh/) or by downloading the debian package on linux.

### Mac

```bash
$ brew tap Oxen-AI/oxen
$ brew install oxen
```

### Debian

```bash
$ wget https://github.com/Oxen-AI/oxen-release/releases/download/v0.4.3/oxen-0.4.3-1-any.deb
$ sudo dpkg -i oxen-0.4.3-1-any.deb
```

## Oxen Server

The Oxen server binary can be deployed where ever you want to store and backup your data. It is an HTTP server that the client communicates with to enable collaboration.

### Mac

```bash
$ brew tap Oxen-AI/oxen-server
$ brew install oxen-server
```

### Docker

```bash
$ wget https://github.com/Oxen-AI/oxen-release/releases/download/v0.4.3/oxen-server-0.4.3.tar
$ docker load < oxen-server-0.4.3.tar
$ docker run -d -v /var/oxen/data:/var/oxen/data -p 80:3001 oxen/hub:0.4.3
```

### Debian

```bash
$ wget https://github.com/Oxen-AI/oxen-release/releases/download/v0.4.3/oxen-server-0.4.3-1-any.deb
$ sudo dpkg -i oxen-server-0.4.3-1-any.deb
```

To get up and running using the client and server, you can follow the [getting started docs](README.md).
