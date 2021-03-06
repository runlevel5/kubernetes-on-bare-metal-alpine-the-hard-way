# Prerequisites

## Alpine Linux

It is required that you have access to computers or VMs running Alpine (edge). It is highly recommended you setup VMs running under VirtualBox or KVM/QEMU.

Please create a normal user and grant full access to this user with `sudo`. A round of Google you could quickly find how to do so.

At the time of the writing, Alpine edge has all the up-to-date kubernetes packages. Please enable Alpine edge repositories:

```sh
echo "http://dl-cdn.alpinelinux.org/alpine/edge/main" | sudo tee /etc/apk/repositories
echo "http://dl-cdn.alpinelinux.org/alpine/edge/community" | sudo tee -a /etc/apk/repositories
echo "http://dl-cdn.alpinelinux.org/alpine/edge/testing" | sudo tee -a /etc/apk/repositories

sudo apk update
sudo apk upgrade
```

Next: [Installing the Client Tools](02-client-tools.md)
