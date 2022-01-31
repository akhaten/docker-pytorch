# docker-pytorch
Install pytorch with docker

---

## Description

docker-pytorch :
- .devcontainer :
    - devcontainer.json : settings for extension vscode in the dev-container
    - Dockerfile : config of container (os, package...)
    - requirements : files having the python libs

---

## Step 1 : Install docker and docker-compose

Link : https://docs.docker.com/get-docker/

NB : You can install with the package manager

### Enable docker

```bash
sudo systemctl enable docker.service
sudo systemctl enable containerd.service

sudo systemctl deamon-reload
sudo systemctl start docker
```

### Add permission

```bash
sudo groupadd docker
sudo usermod -aG docker $USER
```

## Step 2 : Restart machine for update config

## Step 3 : Install and configure vscode

Link : https://code.visualstudio.com/docs/setup/linux

You can install with the package manager (apt, pacman...).

Open vscode and install extension Remote-Container (Ctrl+Shift+X to open extensions manager)

To know more on remote development : https://docs.microsoft.com/en-us/learn/modules/use-docker-container-dev-env-vs-code/

## Step 4 : Put yours files

Copy the files (.ipynb) in the directory docker-pytorch (it's your workspace)


## Step 5 : Build container

Open the folder in a container with Ctrl+Shift+P and `Remote-Containers: Reopen in Containers`. Your workspace is ready ! You can work.


