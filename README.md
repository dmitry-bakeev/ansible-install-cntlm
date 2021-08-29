# Ansible-install-cntlm

## This playbook makes it easy to configure cntlm for isa proxy

You need a remote server in local network with a root user for which the ssh key is added

### How to run

- Set your variables in `group_vars/all.yml`

- `cntlm_username`

- `cntlm_domain`

- `cntlm_password`

- `cntlm_proxy`

- `cntlm_noproxy`

- `cntlm_listen`

- Run this playbook

~~~bash
ansible-playbook -e server_ip=<your-server-ip> -e ssh_private_key_file=<path-to-your-ssh-private-key> setup-cntlm.yml
~~~
