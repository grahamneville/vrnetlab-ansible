# vrnetlab-ansible

Notes:

*Credit to benmaddison whos work inspired me to do this*
*https://github.com/benmaddison/mk-vr-playground/*

If using vEOS then follow my patch to get SSH working:
*https://github.com/plajjan/vrnetlab/pull/166*

Uses Ansible 2.5 and vrnetlab docker containers to spin up a lab environment running BGP with Cisco IOSXE and Arista EOS Devices.
The playbook uses the new network_cli connection methods to connect to the devices.

Running playbook

```
ansible-playbook -i inventory/basic_lab/hosts site.yml
```
