[![Build Status - Master](https://travis-ci.org/juju4/ansible-dc.svg?branch=master)](https://travis-ci.org/juju4/ansible-dc)
[![Build Status - Devel](https://travis-ci.org/juju4/ansible-dc.svg?branch=devel)](https://travis-ci.org/juju4/ansible-dc/branches)

[![Appveyor - Master](https://ci.appveyor.com/api/projects/status/9n7p3hqhb8d4n2aq?svg=true)](https://ci.appveyor.com/project/juju4/ansible-dc)
![Appveyor - Devel](https://ci.appveyor.com/api/projects/status/9n7p3hqhb8d4n2aq/branch/devel?svg=true)

# DetectionLab Windows DC ansible role

Setup a Windows Domain Controller for [DetectionLab](https://github.com/clong/DetectionLab)

WARNING! Work in progress.

## Requirements & Dependencies

### Ansible

Tested with Ansible 2.9

### Operating systems

Targeted for Windows 2016.

### Dependencies

```
$ ansible-galaxy install -r requirements.yml
```

[TODO]

## Example Playbook

Including an example of how to use your role (for instance, with variables
passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - { role: juju4.dc, x: 42 }

You can test with vagrant
```
$ vagrant plugin install vagrant-reload
$ cd test/vagrant
$ vagrant up
$ vagrant provision
$ vagrant ssh
```
Please note that if you run multiple windows VM concurrently, winrm port might change and need to be set manually.

## Continuous integration

This role is tested in Appveyor.

## License

BSD 2-clause
