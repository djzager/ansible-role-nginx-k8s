Role Name
=========

Manages a Nginx application in Kubernetes|OpenShift.

Requirements
------------

* ansible >= 2.6
* [openshift python package](https://pypi.org/project/openshift/)

Role Variables
--------------

See [defaults/main.yml](defaults/main.yml).

Dependencies
------------

None

Example Playbook
----------------

**NOTE** The example below assumes that you have a running Kubernetes|OpenShift
cluster and that you have sufficient permissions in the
`my-nginx-namespace` namespace.

```
- hosts: localhost
  vars:
    name: my-nginx
    namespace: my-nginx-namespace
    size: 3
  roles:
    - name: djzager.nginx_k8s
```
