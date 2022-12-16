# Ansible playbooks to setup a self-hosted WireGuard VPN server

## Usage

```bash
ansible-playbook run.yml -K
```

This repository contains Ansible playbooks to setup a self-hosted WireGuard VPN server. It is based on [wg-easy](https://github.com/WeeJeWel/wg-easy) which provides a nice web interface to add and remove clients.

It also sets up nginx proxy manager so you can access your services from the internet using a domain name.

You can obtain a free domain name from [DuckDNS](https://www.duckdns.org/). You can also use a domain name you already own.
Make sure the domain name is pointing to your server's public IP address.

Then you can use nginx proxy manager to manage your domains and reverse proxy your services.
