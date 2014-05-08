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

TODO: