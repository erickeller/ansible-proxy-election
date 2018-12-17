# Service election over avg rtt

## Goal

One would like to use the service with the least latency from a specific server.

## Ansible version

Due to set_facts with_items bug: https://github.com/ansible/ansible/issues/38991
the version 2.5.1 should be omitted.

## Usage

```
# local example
ansible-playbook -i localhost, -c local election.yml
# remote example
ansible-playbook -i west-server.example.com, --private-key ~/.ssh/id_rsa -u test election.yml
```
