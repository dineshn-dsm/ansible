# Deploy sample LAMP stack application using ansible playbook

Playbook will install below packages and creates DB and imports sample data and clone sample code from github.

Note: package works for Ubuntu, working for other LInux os family.


## Resources


These types of resources are supported:

* [apt]
* [service]
* [mysql_db]
* [mysql_user]
* [file]
* [git]
* [replace]

## Ansible versions

ansible 2.9.6

## Usage

Install ansible --> clone this repo --> update  required input values --> Run below commands

ansible-playbook LAMP-stack_app-deploy.yml


## Changes required

comment below value in playbook if using different host to install

```yml
login_unix_socket: /var/run/mysqld/mysqld.soc
```



## Notes

package works for Ubuntu, working for other LInux os family.


## Requirements
NA
## Modules

No external Modules.

## Inputs

| Name | Description | Type | Default | Required |
|------|-------------|------|---------|:--------:|


## Outputs

1. curl http://localhost

## Revert changes

ansible-playbook LAMP-stack_app-remove.yml

## Author

Managed by [Dinesh N](https://github.com/dineshn-dsm).
