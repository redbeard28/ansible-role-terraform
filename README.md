ansible-role-terraform
========

Ansible role to install Terraform on Linux and Darwin machines.

## Compatibility ?



## Howto use this role?
This role need to be include in a playbook. 

Call this **Galaxy** role  like this:

````bash
ansible-galaxy install -r requirements.yml 
````

Inside requirements.yml
````yaml
# from GitHub, overriding the name and specifying a specific tag
- src: git+https://github.com/redbeard28/ansible-role-terraform.git
  version: master
  name: terraform
````

or
````yaml
# from Ansible-Galaxy
- src: redbeard28.terraform
````

More info => [Ansible Docs](https://docs.ansible.com/ansible-container/roles/access.html)

## Requirements

 * Ansible 2.8+



Role Variables
--------------

Here are the role variables and their default values. Default password for user terraform is terraform.
```
terraform_version: 0.12.19
terraform_dir: /user/local/bin/terraform
terraform_user: terraform
terraform_user_password: $6$uoCgixKJL4cFyIT$U7FisaA6GAdosBpGde.4NS00vaAg4tGmR63eBQQMsd8LiHUjetq6HDXG10719JwbNmQUSLzvG6zq8DOVOggIw1
```

Example Playbook
-------------------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

```
- hosts: all
  roles:
    - role: redbeard28.terraform
```

License
-------

GPLv3

Author Information
------------------

by [Jeremie CUADRADO](https://github.com/redbeard28)
