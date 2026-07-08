
# Custom Ansible Image

## Repo
https://github.com/gatomek/docker-ansible

## Description
Image prepared as a tool for easy upload applications and configurations to cloud infrastructure. 
No need for Linux OS or WSL.

## Content
- base image: alpine/ansible:2.21.0
- known_hosts file prepared
- priv key added (local usage only)

## Building the image
```sh
docker image build --tag gatomek_ansible .
```

## Backlog
- [ ]  Image without priv key. Use alternative way of usage the priv key without having them in image layer. 

