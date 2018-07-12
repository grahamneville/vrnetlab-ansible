# vrnetlab-ansible

Notes:

*Credit to benmaddison whos work inspired me to do this*
*https://github.com/benmaddison/mk-vr-playground/*

vrnetlab now includes my patch to get SSH working on vEOS:
*https://github.com/plajjan/vrnetlab/pull/166*

VxLan Lab:
- Features 2 Spine switches, 2 Leaf switches, 2 End Hosts
- End Hosts are just vEOS devices
- End Host1 connected to Leaf1
- End Host2 connected to Leaf2
- VxLAN didn't work in 4.20.1F, used 4.20.7M - also Layer3 interfaces have to have a high MTU set

Uses Ansible 2.5 and vrnetlab docker containers to spin up a lab environment running BGP with Cisco IOSXE and Arista EOS Devices.
The playbook uses the new network_cli connection methods to connect to the devices.

Running playbook examples:

```
ansible-playbook -i inventory/basic_lab/hosts site.yml
```

```
ansible-playbook -i inventory/leaf_spine_basic/hosts site.yml
```
