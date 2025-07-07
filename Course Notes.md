# Course Notes for Building a Home IT Lab

This document contains notes for the course _Building a Home IT Lab_, which is available on LinkedIn Learning.

## Sample Lab Configurations

This table shows which products are used in the course, and how their sample lab is set up.

| **Type**       | **Product**               | **Guests or Services**          | **Network**                       |
| -------------- | ------------------------- | ------------------------------- | --------------------------------- |
| Infrastructure | Hyper-V                   | Ubuntu Server<br>Ubuntu Desktop | Shared private network            |
| Infrastructure | Proxmox VE (KVM)          | Ubuntu Server<br>Ubuntu Desktop | Bridged adapter to host's network |
| Infrastructure | XCP-ng (Xen)              | Ubuntu Server<br>Ubuntu Desktop | Shared private network            |
| Desktop        | VirtualBox                | Ubuntu Server<br>Ubuntu Desktop | Bridged adapter to host's network |
| Desktop        | QEMU with KVM             | Ubuntu Server<br>Ubuntu Desktop | Individual private networks       |
| Desktop        | Virtual Machine Manager   | Ubuntu Server<br>Ubuntu Desktop | Shared private network            |
| Container      | LXC                       | Ubuntu Linux                    | Shared private network            |
| Container      | Docker                    | Alpine Linux                    | Shared private network            |
| Storage        | TrueNAS Community Edition | SMB/ZFS storage                 | Host                              |

## Ubuntu Desktop and Ubuntu Server

Installer ISOs are available from [ubuntu.com/download](https://www.ubuntu.com/download).

## Hyper-V

Enable Hyper-V on a supported Windows system by checking the appropriate box in the _Turn Windows Features On or Off_ menu.

[Microsoft Learn: Virtualization documentation](https://docs.microsoft.com/en-us/virtualization)

## Proxmox VE

Installer ISO is available from [proxmox.com](https://www.proxmox.com).

Note: if you have an NVIDIA GPU, you may need to add `nomodeset` to the installer's boot configuration to avoid a freeze during installation.

See [Proxmox Virtual Environment Essential Training]() on LinkedIn Learning for more details.

## XCP-ng

Installer ISO is available from [xcp-ng.org](https://www.xcp-ng.org).

[Xen Project Wiki: Getting Started](https://wiki.xenproject.org/wiki/Getting_Started)

[Xen Orchestra](https://www.xen-orchestra.com)

## VirtualBox

Installer is available from [virtualbox.org](https://www.virtualbox.org).

See [Learning VirtualBox](https://www.linkedin.com/learning/learning-virtualbox-19862434) on LinkedIn Learning for more details.

## KVM and QEMU

Install with `apt install qemu-system-x86` or with your distro's package manager. Emulators for other architectures are also available.

See [Virtualization with KVM and Qemu](https://www.linkedin.com/learning/virtualization-with-kvm-and-qemu) on LinkedIn Learning for more details.

## Virtual Machine Manager

Install with `apt install virt-manager` or with your distro's package manager.

## TrueNAS Community Edition Notes

Installer ISO is available from [truenas.com](https://www.truenas.com).

Remember: Use storage other than the boot pool for shared files, virtual machines, containers, and apps.

## Linux Containers

Install LXD on an Ubuntu system with `snap install lxd`.

Read more about Linux Containers at [linuxcontainers.org](https://www.linuxcontainers.org).

## Docker

Install Docker with `apt install docker.io` or with your distro's package manager.

See [Learning Docker](https://www.linkedin.com/learning/learning-docker-17236240) on LinkedIn Learning for more details.

## Additional LinkedIn Learning Courses

[Learning Virtualization](https://www.linkedin.com/learning/learning-virtualization-13945890)

[DevOps Foundations: Containers](https://www.linkedin.com/learning/devops-foundations-containers-14207858)

[Networking Foundations: IP Addressing](https://www.linkedin.com/learning/networking-foundations-ip-addressing-2020)
