# Overview
This role is to install the base requirements on an Ubuntu system in order to manage it via puppet.
## Installation
This role is the equivilent of running:

```
sudo apt update
sudo apt install virtualenv python-pip -y
sudo apt install docker.io -y
pip install docker
```
## Assumptions
This role assumes that the latest versions of all downloaded software is compatible.
