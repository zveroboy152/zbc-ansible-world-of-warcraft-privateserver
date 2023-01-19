# README.md

## Deploy TrinityCoreDocker (by cbrgm / cmangos-docker)

This repository contains an Ansible playbook to deploy TrinityCoreDocker on a production server. The playbook uses the source from https://github.com/cbrgm/cmangos-docker, a repository containing the TrinityCoreDocker files.

The playbook includes the following tasks:

1. Installing software dependencies such as git, docker.io, docker-compose, glances, wget, htop, and nano.

2. Creating a directory at /tmp/wow if it does not exist.

3. Cloning a Github repository containing the TrinityCoreDocker files to /tmp/wow.

4. Running the `docker-compose up -d` command to deploy the TrinityCoreDocker server.

### Usage

To use this playbook, you will need to have Ansible installed on your machine and configure the `hosts.yaml` file to target your production server. Then, you can run the playbook with the command `ansible-playbook -i hosts deploy_trinitycoredocker.yaml`.
