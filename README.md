Netplan
=========

Simple role to manage netplan config files and apply them.


Role Variables
--------------

This roles takes the variable `netplan_config` as input to generate the files as defined. As you can see in the following code block example,
`netplan_config` is a dictionary, where each key represents a netplan config file in `/etc/netplan/` and each value of those keys represents the config written in each file.

```yaml
netplan_config:
  50-cloud-init:
    network:
      ethernets:
        enp0s3:
          dhcp4: true
          match:
            macaddress: 02:74:c4:98:7d:21
          set-name: enp0s3
      version: 2
  50-vagrant:
    network:
      version: 2
      renderer: networkd
      ethernets:
        enp0s8:
          addresses:
            - 192.168.7.19/24
```

Dependencies
------------

None

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
