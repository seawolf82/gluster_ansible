# gluster_ansible

This script install glusterfs on Redhat based Distributions

Tested on:

- RockyLinux 8
- RockyLinux 9
- Centos 7

Tested on:

- 2.9 Ansible version

To install Gluster run:
ansible-playbook -vv -i hosts site.yaml

To uninstall Gluster run:
ansible-playbook -vv -i hosts deprovision.yaml

Adding Tags to permit run only specific task of playbook

Tags:

upgrade
package
ntp
gluster


For example, to launch only task regarding upgrade os, run:
 
ansible-playbook -vv --tags "upgrade" -i hosts site.yaml
