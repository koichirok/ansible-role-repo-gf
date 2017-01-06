Role Name
=========

Installs [Ghettoforge](http://ghettoforge.org/index.php/Main_Page) repository for RHEL/CentOS.

Requirements
------------

None.

Role Variables
--------------

Availabe role variables are listed below, along with default values:

```yaml
repo_gf_release_ver: 10

repo_gf_enable_repos:
  - "gf"
```

`repo_gf_release_ver` is variable to specify gf repo's release version.

`repo_gf_enable_repos` is variable to specify repositories which you want to enable by default.
 Possible values: gf, gf-plus, gf-testing, gf-source, gf-plus-source, gf-testing-source

Dependencies
------------

None.

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

CC0
