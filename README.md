Load Balancer
=============

Sets up a Haproxy software load balancer to redirect http traffic to https and relay the SSL traffic to load balanced SSL-enabled backends.

Role Variables
--------------

- `backends` - A list of IPs from the backend servers to be load balanced, these will usually be local IPs. Declared but undefined, it is expected to be defined on `vars/main.yml` or overriden on the global scope.

Dependencies
------------

The [common role](https://git.forgeservicelab.fi/ansible-roles/common) is defined as a dependency, make sure it is present in your playbook.

Author Information
------------------

[Forge Servicelab Team](http://forgeservicelab.fi)
