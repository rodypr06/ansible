linux rootpassword
=========

# [![Build Status](https://travis-ci.org/ANTS-Framework/linux_rootpassword.svg?branch=master)](https://travis-ci.org/ANTS-Framework/linux_rootpassword)

Set the root password using the ansible [user module](http://docs.ansible.com/ansible/latest/user_module.html).

Password hashes for most linux distributions can be generated as documented
[here](http://docs.ansible.com/ansible/latest/faq.html#how-do-i-generate-crypted-passwords-for-the-user-module)

Role Variables
--------------

```yml
    linux_rootpassword__password: 'plz_change_me'
```

Example Playbook
----------------

```yml
    - hosts: classroom
      vars:
        - linux_rootpassword__password: "hashvaluehere"
      roles:
        - linux_rootpassword
```

License
-------

GPLv3

Author Information
------------------
Part of the [ANTS Framework](https://ants-framework.github.io/)
