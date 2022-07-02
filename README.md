# Simple Ansible Playbook collections

It's a simples collection of playbooks I developed on my work to accomplish some tasks on my daily work.

All playbook here are built to run on systems based on RHEL.

We adopt [AlmaLinux](https://almalinux.org/) as default for our systems but all RHEL 8 like or higher it should be run as well.

# [NGINX](nginx.yml)

Installing the latest NGINX version for RHEL, configure firewalld to open HTTP and HTTPS port and allow SELinux to connect through HTTP.

```
ansible-playbook nginx.yml
```
