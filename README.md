[![License](https://img.shields.io/badge/license-Apache%202-blue.svg)](https://www.apache.org/licenses/LICENSE-2.0)

======================

Ansible Role to install an HTCondor [HTCondor] Cluster (https://research.cs.wisc.edu/htcondor/).
Forked from grycap version

Role Variables
--------------

The variables that can be passed to this role and a brief description about them are as follows.
```
# Type of node to install: front or wn
htcondor_type_of_node: front
# Prefix to set to the HTcondor working nodes
htcondor_vnode_prefix: wn
# Default ssh user
htcondor_ssh_user: grycap
# Number of Maximum nodes
max_number_of_nodes: 3
```

Example Playbook
----------------

This an example of how to install an HTCondor cluster with three nodes:
```
- hosts: server
  roles:
  - { role: 'grycap.htcondor', htcondor_type_of_node: 'front' }
```
Contributing to the role
========================
In order to keep the code clean, pushing changes to the master branch has been disabled. If you want to contribute, you have to create a branch, upload your changes and then create a pull request.
Thanks
