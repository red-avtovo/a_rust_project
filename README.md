# A rust project

This is a wrapper which allows to develop and build any project on a remote machine with SSH access and installed Docker thanks to VS Code Remote Containers plugin

## How to use

* Get a remote machine with installed Docker
* Generate a ssh-id rsa key with `ssh-keygen`
* Copy ssh id to it to with `ssh-copy-id`

On remote machine:
* Clone the project you want to work with

On local machine:
* Change `docker.host` in `.vscode/settings.json`
* Open this project in VS Code
* Provide absolute path of cloned project on remote machine in parameter `workspaceMount` in file `.devcontainer/devcontainer.json`
* Keep as it is or change the docker image where you want to build the project in `.devcontainer/devcontainer.json`, parameter `image` or build you own Docker image uncommentin dockerFile property
* Run command: `Remote-containers: Reopen in Container`
* Wait a bit
* Start coding :)

ref: https://code.visualstudio.com/docs/remote/containers

## Not Rust project

Just opdate recomended extensions and base image and use it as another-language remote project

Support the project: [![Donate button](https://www.paypalobjects.com/en_US/DK/i/btn/btn_donateCC_LG.gif)](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=H337RKJSC4YG4&source=url)
