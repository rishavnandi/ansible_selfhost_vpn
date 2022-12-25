# Ansible playbooks to setup a self-hosted WireGuard VPN server

![Screenshot (1)](https://user-images.githubusercontent.com/101431112/209468911-88c70c8d-c686-4dac-b4c7-bc3b1fb67568.png)

## Usage

- Clone the repo 
```bash
git clone https://github.com/rishavnandi/ansible_selfhost_vpn
```
- Then modify the variables in the group_vars/all/vars.yml based on your needs and add your server's IP and path of the ssh key(if you are using one) in the inventory file 

- Then simply run the playbook
```bash
ansible-playbook run.yml -K
```
- Then you can visit the nginx proxy manager at your server's IP and port 81 to configure a domain that points to nginx and WireGuard sites

## References and Info

This repository contains Ansible playbooks to setup a self-hosted WireGuard VPN server. It is based on [wg-easy](https://github.com/WeeJeWel/wg-easy) which provides a nice web interface to add and remove clients.

It also sets up nginx proxy manager so you can access your services from the internet using a domain name.

You can obtain a free domain name from [DuckDNS](https://www.duckdns.org/). You can also use a domain name you already own.
Make sure the domain name is pointing to your server's public IP address.

Then you can use nginx proxy manager to manage your domains and reverse proxy your services.
