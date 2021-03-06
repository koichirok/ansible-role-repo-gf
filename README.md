koichirok.repo-gf
=========

[![Travis](https://travis-ci.org/koichirok/ansible-role-repo-gf.svg?branch=master)](https://travis-ci.org/koichirok/ansible-role-repo-gf)
[![Ansible Role](https://img.shields.io/ansible/role/14693.svg)](https://galaxy.ansible.com/koichirok/repo-gf/)

Installs [Ghettoforge](http://ghettoforge.org/index.php/Main_Page) repository for RHEL/CentOS.

Role Variables
--------------

Availabe role variables are listed below, along with default values:

```yaml
repo_gf_enable_repos:
  - "gf"
```

`repo_gf_enable_repos` is variable to specify repositories which you want to enable by default.
 Possible values: gf, gf-plus, gf-testing, gf-source, gf-plus-source, gf-testing-source

Example Playbook
----------------

```yaml
- hosts: servers
  roles:
     - role: koichirok.repo-gf
       repo_gf_enable_repos:
         - "gf-testing"
```

License
-------

[CC0-1.0](./LICENSE)
