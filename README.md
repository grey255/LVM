# lvm_role
=========

This role creates and mounts a file system.<br>

# Requirements
------------

 * Two servers (virtual machines) i.e. database2.nextgenlabs.com and dns2.nextgenlabs.com<br>
 * Each server should have an unused block device /dev/sdb (or other forms of devices)
 * Volume group: vg.alzheimers<br>
 * Logical volume: lv.alzheimers<br>

# Role Variables
--------------
 * All variables defined in vars/main.yaml <br>

# Dependencies
------------
 * Mounting done using UUID<br>
 

# Example Playbook
----------------

    ---
    - name: play does logical volume management
      hosts: all
      become: true
      roles:
         - lvm_role

License
-------

BSD

Author Information
------------------

grey deegaines06@gmail.com
