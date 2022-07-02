# Simple Ansible Playbook collections

It's a simples collection of playbooks I developed on my work to accomplish some tasks on my daily work.

All playbook here are built to run on systems based on RHEL.

We adopt [AlmaLinux](https://almalinux.org/) as default for our systems but all RHEL 8 like or higher it should be run as well.

The [hosts](hosts) contains a basic structure I used to use for control the execution of my playbooks.

# [NGINX](nginx.yml)

Installing the latest NGINX version for RHEL, configure firewalld to open HTTP and HTTPS port and allow SELinux to connect through HTTP.

```
ansible-playbook -i hosts nginx.yml
```

# [Zabbix Server](zabbix-server.yml)

Installing Zabbix Server and frontend including service along side with a NGINX virtualhost and PHP-FPM socket.

```
ansible-playbook -i hosts zabbix-server.yml
```

# [Zabbix Agent](zabbix-agent.yml) for RHEL

Installing Zabbix Agent for systems based on RHEL 8.

```
ansible-playbook -i hosts zabbix-agent.yml
```

# [Zabbix Agent Legacy](zabbix-agent-legacy.yml) for RHEL 5, 6 or 7

Installing Zabbix Agent for systems based on RHEL 5, 6 or 7 like.

```
ansible-playbook -i hosts zabbix-agent-legacy.yml
```
