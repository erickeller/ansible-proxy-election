# Service election over avg rtt

## Goal

One would like to use the service with the least latency from a specific server.

## Usage

```
# local example
ansible-playbook -i localhost, -c local election.yml
# remote example
ansible-playbook -i west-server.example.com, --private-key ~/.ssh/id_rsa -u test election.yml
```
