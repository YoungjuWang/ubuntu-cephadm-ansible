# ubuntu-cephadm-ansible

Deploy ssh-key to hosts in advance.

1. Edit inventory file
2. Check connection via ansible ping module / ex) ansible -m ping -i ceph.inventory all 
3. Run preflight ansible-playbook
```
# ansible-playbook -i ceph.inventory preflight.yml
```

