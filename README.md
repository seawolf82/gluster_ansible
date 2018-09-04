# gluster_ansible

This script install glusterfs 4.1 on centos 7 

To install Gluster 4.1 run:
ansible-playbook -vv -i hosts site.yaml

To uninstall Gluster 4.1 run:
ansible-playbook -vv -i hosts deprovision.yaml

Adding Tags to permit run only specific task of playbook

Tags:

upgrade
package
ntp
gluster


For example, to launch only task regarding upgrade os, run:
 
ansible-playbook -vv --tags "upgrade" -i hosts site.yaml
