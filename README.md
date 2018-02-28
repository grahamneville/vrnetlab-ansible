# vrnetlab-ansible

Uses Ansible 2.5 and vrnetlab docker containers to spin up a lab environment running BGP with Cisco IOSXE and Arista EOS Devices.
The playbook uses the new network_cli connection methods to connect to the devices.

TODO:
 - Work out how to pass a list to vr-xcon instead of static entries


Running playbook

```
ansible-playbook -i inventory/basic_lab/hosts site.yml
```
