# Ansible roles collection

## Usage

### Configuration

For use a custum role path:

create a file `ansible.cfg` in directory where ansible run

ansible.cfg:
````
# config file for ansible -- http://ansible.com/
# ==============================================

# nearly all parameters can be overridden in ansible-playbook
# or with command line flags. ansible will read ANSIBLE_CONFIG,
# ansible.cfg in the current working directory, .ansible.cfg in
# the home directory or /etc/ansible/ansible.cfg, whichever it
# finds first

[defaults]

# additional paths to search for roles in, colon seperated
roles_path    = ansible-roles
````

## In a project 

### in git project

`git submodule add git@github.com:aarnaud/ansible-roles.git ansible-roles`

### in other project 

 `git clone git@github.com:aarnaud/ansible-roles.git ansible-roles`

### first playbook:

myplaybook.yml:
````
---

- name: First exemple
  hosts: all
  user: root

  roles:
    - common
    - nginx
    - nodejs
    - shorewall
````
