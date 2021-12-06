# ubuntu-cephadm-ansible

Deploy ssh-key to hosts in advance.

1. Edit inventory file
2. Check connection via ansible ping module `ansible -m ping -i ceph.inventory all`
3. Edit `vars.yml` file
```
container_engine: "podman" or "docker"
ceph_origin: 'community' or 'testing'
ceph_release: 'pacific' or Others
timezone: 'Asia/Seoul' or Others
ntp_server: '0.kr.pool.ntp.org' or Others
```
4. Run `preflight` ansible-playbook
```
# ansible-playbook -i ceph.inventory preflight.yml
```

