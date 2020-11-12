# dev-containers

Docker images for easy setup of local development and build environments.

Box setups for:

- [Ansible](ansible/Dockerfile)

## Requirements

- Docker

## How to Build

    docker build . -t ansible:latest

## How to Run

    docker run -it --rm --volume %cd%:/ansible -w /ansible ansible

## License

[MIT](LICENSE)

## Author Information

Created by [Philippe Bößling](https://www.gihub.com/pboessling).
