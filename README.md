# Deploy sample LAMP stack application using ansibl playbook on Ubuntu

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

## Terraform versions

ansible 2.9.6

## Usage

Install ansible --> clone this repo --> update  required input values --> Run below commands

ansible-playbook kodecloud-ecomm-app.yml


## Changes required

comment below value in playbook if using different host to install

```yml
login_unix_socket: /var/run/mysqld/mysqld.soc
```



## Notes

package works for Ubuntu, working for other LInux os family.


<!-- BEGINNING OF PRE-COMMIT-TERRAFORM DOCS HOOK -->
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

ansible-playbook sample_LAMP-stack_app-remove.yml

## Author

Module managed by [Dinesh N](https://github.com/dineshn-dsm).
