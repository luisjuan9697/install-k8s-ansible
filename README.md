# Overview
An Ansible playbook that installs Kubernetes.



# Features
- containerd
- calico for pod networking

# Quickstart
```
ansible -i inventory/dev all -m ping

ansible-playbook -i inventory/dev playbooks/k8s_all.yaml

# reboot might be required after installation
ansible -i inventory/dev all -a "/sbin/reboot" --become
```
