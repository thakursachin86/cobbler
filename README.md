
# Cobbler Batch Installation

> This is a cobbler platform that runs in docker.

### File Description

Build a Cobbler Mirrored Dockerfile:

- Dockerfile
- start.sh

Compose dockerfile running cobbler container:

- docker-compose.yml
- cobbler.env

### Instructions for use

1. first change the variable information in the `cobbler.env` variable file
2. the system image is mounted to the machine's `/mnt` directory
3. Run the cobbler container: `docker-compose up -d`
4. into the cobbler container, configure the installed system: `docker exec -it dockercobbler_cobbler_1 bash`
