Containerization OverlayFS
=========


* Galaxy: [![Ansible Galaxy](https://img.shields.io/badge/galaxy-tcharl.ansible_containerization-660198.svg?style=flat)](https://galaxy.ansible.com/tcharl/ansible_containerization)
* Lint & requirements: ![Molecule](https://github.com/OsgiliathEnterprise/ansible-containerization/workflows/Molecule/badge.svg)
* Tests: [![Build Status](https://app.travis-ci.com/OsgiliathEnterprise/ansible-containerization.svg?branch=master)](https://travis-ci.com/OsgiliathEnterprise/ansible-containerization)
* Chat: [![Join the chat at https://gitter.im/OsgiliathEnterprise/platform](https://badges.gitter.im/OsgiliathEnterprise/platform.svg)](https://gitter.im/OsgiliathEnterprise/platform?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)

This role enriches the original [geerlinguy docker role](https://github.com/geerlingguy/ansible-role-docker) and use the [Ansible volumes plus](https://github.com/OsgiliathEnterprise/ansible-volumes) role in order to add overlayfs driver support configuration for docker. Also configures lvms and volumes for docker.

Requirements
------------

Tox python 3.6+ and Ansible 2.9+ are required to run the tests.

Test
--------------

1. Install the dependencies with `tox -e pipdeps`
2. Run the tests with `tox -e testexec --scenario-name <your virtualization hypervisor>`

   For example, to run the tests with Vagrant and kvm, you can use:

   ```bash
   tox -e testexec --scenario-name kvm
   ```

   Or to run the tests with parallels, you can use:

   ```bash
   tox -e testexec --scenario-name parallels
   ```

Role Variables
--------------

Only [dependencies variables](https://github.com/OsgiliathEnterprise/ansible-containerization/blob/master/molecule/default/molecule.yml) at all but those of the dependencies, see [molecule tests](https://github.com/OsgiliathEnterprise/ansible-containerization/blob/master/molecule/default/tests/test_default.py) for more info.

Dependencies
------------

As said
 * [geerlinguy docker role](https://github.com/geerlingguy/ansible-role-docker)
 * [Ansible volumes](https://galaxy.ansible.com/tcharl/ansible_volumes)

Example Playbook
----------------

See the [vars declared](https://github.com/OsgiliathEnterprise/ansible-containerization/blob/master/molecule/default/molecule.yml) on the molecule test, as well as [their impact](https://github.com/OsgiliathEnterprise/ansible-containerization/blob/master/molecule/default/tests/test_default.py) 


License
-------

[Apache-2](https://www.apache.org/licenses/LICENSE-2.0)

Author Information
------------------

* Twitter [@tcharl](https://twitter.com/Tcharl)
* Github [@tcharl](https://github.com/Tcharl)
* LinkedIn [Charlie Mordant](https://www.linkedin.com/in/charlie-mordant-51796a97/)
