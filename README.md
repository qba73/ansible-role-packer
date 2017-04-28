Role Name
=========

Ansible role for installing Packer.

Requirements
------------

CentOS / RedHat 7 

Role Variables
--------------

    - packer_ver: <version> 
    - packer_checksum: <checksum> 
    - packer_dest_path: /usr/local/bin
    - packer_dest_link: /usr/bin


Dependencies
------------

Unzip package will be installed if it's not installed already.

Example Playbook
----------------

How to use the role with default params:

    - hosts: servers
      roles:
         - { role: packer }


How to use the role to install specific version of Packer:

    - hosts: servers
      roles:
         - { role: packer, packer_ver: 0.12.2, packer_checksum: 035d0ea1fe785ab6b673bc2a79399125d4014f29151e106635fa818bb726bebf }

Checksums can be downloaded from [packer.io page](https://releases.hashicorp.com/packer/).


Author Information
------------------

todo

