# Percona + Nginx(Test) + Keepalived + HAProxy (2 Nodes)

# Usage
- Change node ips in hosts file
- Change your variables in defaults
- `ansible-playbook -i hosts site.yml`

# How to restart the cluster nodes

- In Node2 `systemctl stop mysql`
- In Node1 `systemctl stop mysql@bootstrap`
- Restart Nodes and start **mysql@bootstrap** in Node1 and **mysql** in Node2