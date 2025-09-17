# Laravel Docker Installer

[![Requires Docker](https://img.shields.io/badge/prerequisite-Docker-blue)](https://www.docker.com)
[![Docker Pulls](https://img.shields.io/docker/pulls/krajbanshi/laravel-docker.svg)](https://hub.docker.com/r/krajbanshi/laravel-docker)
![Docker Image Version](https://img.shields.io/docker/v/krajbanshi/laravel-docker?label=version&logo=docker)
[![Docker Image Size](https://img.shields.io/docker/image-size/krajbanshi/laravel-docker)](https://hub.docker.com/r/krajbanshi/laravel-docker)
[![GitHub License](https://img.shields.io/github/license/kishor-rajbanshi/laravel-docker-installer)](./LICENSE)

This repository contains the source code for the **Laravel Docker Installer**.
The installer is available as a prebuilt Docker image on [Docker Hub](https://hub.docker.com/r/krajbanshi/laravel-docker).
It is designed to quickly set up the [Laravel Docker package](https://github.com/kishor-rajbanshi/laravel-docker) in your project.

---

## 🔗 Quick Links

- 📦 [Laravel Docker Package](https://github.com/kishor-rajbanshi/laravel-docker)
- 🐳 [Docker Hub: Installer Image](https://hub.docker.com/r/krajbanshi/laravel-docker)
- 💻 [Installer Source Repository](https://github.com/kishor-rajbanshi/laravel-docker-installer)

---

## Installation

Pull the installer image:

```sh
docker pull krajbanshi/laravel-docker
````

You can also pull a specific version:

```sh
docker pull krajbanshi/laravel-docker:<tag>
```

---

## Usage

Once the installer image is pulled, you can use it to set up the [Laravel Docker package](https://github.com/kishor-rajbanshi/laravel-docker) in your project.

### Unix Shell (Linux / macOS)

```sh
docker run --rm -v "$(pwd):/app" -u "$(id -u):$(id -g)" krajbanshi/laravel-docker
```

### PowerShell (Windows)

```powershell
docker run --rm -v "${PWD}:/app" krajbanshi/laravel-docker
```

### CMD (Windows)

```cmd
docker run --rm -v "%cd%:/app" krajbanshi/laravel-docker
```

### Install a Specific Version

To install a specific version, just pass it as an argument:

```sh
docker \
    run \
    --rm \
    -v "$(pwd):/app" \
    -u "$(id -u):$(id -g)" \
    krajbanshi/laravel-docker <version>
```

---

## Notes

- This repository contains the **installer source code** used to build the image published on Docker Hub.
- The **Laravel Docker package** itself is maintained in a separate repository.
- Contributions and issues related to the installer should be opened here.

---

## License

[MIT](./LICENSE)
