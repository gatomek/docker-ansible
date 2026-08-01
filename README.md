
# Custom Ansible Image

## Repo
https://github.com/gatomek/docker-ansible

## Description
Image prepared as a tool for easy upload applications and configurations to cloud infrastructure. 
No need for Linux OS or WSL during development.

## Content
- base image: alpine/ansible:2.21.0
- known_hosts file prepared
- priv key added (local usage only)

## Building the image locally (Docker Desktop)
```sh
docker image build --tag registry.gatomek.pl/projects/ansible .
```

## Building the image on Tower
```sh
docker --context docker-on-tower image build --add-host tower=192.168.18.238 --tag registry.gatomek.pl/projects/ansible .
```

## Backlog
- [ ]  Image without priv key. Use alternative way of usage the priv key without having them in image layer. 

## Remarks
* registry `registry.gatomek.pl/projects/` does not exist
* image name `registry.gatomek.pl/projects/ansible` is a security name against accidentally pushing image to remote registry
