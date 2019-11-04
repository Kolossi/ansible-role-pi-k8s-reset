Ansible Role : Raspberry Pi4 Kubenetes reset
=========

This role will reset a kubernetes cluster installed on a master and multiple
workers, and uninstall kubernetes and docker..

Expected use case is after successful or partial installation of kubernetes 
with [pi-k8s_playbook.yml](https://github.com/Kolossi/ansible-role-pi-k8s), to
reset to try again.

Hosts file
----------

An example hosts file is provided in this directory, uncomment and edit for
ip addresses and number of workers.

Example Playbook
----------------

An example playbook `pi-k8s-reset_playbook.yml` is provided in this directory.

To use, run:
```
ansible-playbook pi-k8s-reset_playbook.yml
```

To limit to certain hosts use e.g.
```
ansible-playbook pi-k8s-reset_playbook.yml -l k8s-pi-master
```

License
-------

GPL v3.0

