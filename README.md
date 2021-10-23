# Ansible Role: Docker

An Ansible Role that installs [Docker](https://www.docker.com) on Linux.

## Requirements

None.

## Role Variables

    docker_edition: 'ce'
    docker_package: "docker-{{ docker_edition }}"
    docker_package_state: present
    docker_service_state: started
    docker_service_enabled: true
    docker_restart_handler_state: restarted
    docker_install_compose: true
    docker_compose_version: "1.26.0"
    docker_compose_path: /usr/local/bin/docker-compose
    docker_repo_url: https://download.docker.com/linux
    docker_users:
      - user1
      - user2
A list of system users to be added to the `docker` group (so they can use Docker on the server).

## Dependencies

None.
