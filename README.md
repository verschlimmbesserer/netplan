Role Name
=========

A brief description of the role goes here.

Requirements
------------

Any pre-requisites that may not be covered by Ansible itself or the role should be mentioned here. For instance, if the role uses the EC2 module, it may be a good idea to mention in this section that the boto package is required.

Role Variables
--------------

A description of the settable variables for this role should go here, including any variables that are in defaults/main.yml, vars/main.yml, and any variables that can/should be set via parameters to the role. Any variables that are read from other roles and/or the global scope (ie. hostvars, group vars, etc.) should be mentioned here as well.
```yaml
netplan_config: {}
#  50-cloud-init:
#    network:
#      ethernets:
#        enp0s3:
#          dhcp4: true
#          match:
#            macaddress: 02:74:c4:98:7d:21
#          set-name: enp0s3
#      version: 2
#  50-vagrant:
#    network:
#      version: 2
#      renderer: networkd
#      ethernets:
#        enp0s8:
#          addresses:
#            - 192.168.7.19/24
```




Dependencies
------------

A list of other roles hosted on Galaxy should go here, plus any details in regards to parameters that may need to be set for other roles, or variables that are used from other roles.

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - { role: username.rolename, x: 42 }

License
-------

GNU General Public License v3.0

Author Information
------------------

An optional section for the role authors to include contact information, or a website (HTML is not allowed).
