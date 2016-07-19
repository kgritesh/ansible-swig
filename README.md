Role Name
=========

This role downloads and installs swig library. User can configure the version of
the library using variables


Role Variables
--------------

The variables that can be passed to this role and a brief description about
them are as follows. (For all variables, take a look at [defaults/main.yml](defaults/main.yml))

```yaml

swig_version: "3.0.10" # Swig version that needs to be installed

swig_mirror: "http://ufpr.dl.sourceforge.net/project/swig/swig" # Swig mirror

swig_dependencies_debian: [] # List of swig dependencies for debian

swig_dependencies_redhat: [] # List of swig dependencies for redhat

swig_dir: '/opt/swig' # Path to install swig

tmp_dir: '/tmp' # Path to initially download swig

```


Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - { role: kgritesh.ansible-swig, swig_ver: 3.10 }

License
-------

BSD

