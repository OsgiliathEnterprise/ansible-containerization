Docker OverlayFS
=========

This role enriches the original [crivetimihai virtualization collection docker role](https://github.com/crivetimihai/ansible_virtualization/tree/master/roles/docker) and use the [Ansible manage lvm plus](https://github.com/OsgiliathEnterprise/ansible-manage-lvm-plus) role in order to add overlayfs driver support configuration on docker

Requirements
------------

You should first execute `./configure` first, which will download the requirements in siblings folders

Role Variables
--------------

Only [dependencies variables](https://github.com/OsgiliathEnterprise/ansible-docker/blob/master/molecule/default/molecule.yml) at all but those of the dependencies, see [molecule tests](https://github.com/OsgiliathEnterprise/ansible-docker/blob/master/molecule/default/tests/test_default.py) for more info.

Dependencies
------------

As said
 * [crivetimihai virtualization collection](https://galaxy.ansible.com/crivetimihai/virtualization)
 * [Ansible manage lvm plus](https://galaxy.ansible.com/tcharl/ansible_manage_lvm_plus)

Example Playbook
----------------

See the [vars declared](https://github.com/OsgiliathEnterprise/ansible-docker/blob/master/molecule/default/molecule.yml) on the molecule test, as well as [their impact](https://github.com/OsgiliathEnterprise/ansible-docker/blob/master/molecule/default/tests/test_default.py) 


License
-------

[Apache-2](https://www.apache.org/licenses/LICENSE-2.0)

Author Information
------------------

Twitter [@tcharl](https://twitter.com/Tcharl)
Github [@tcharl](https://github.com/Tcharl)
LinkedIn [Charlie Mordant](https://www.linkedin.com/in/charlie-mordant-51796a97/)
