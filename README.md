# terraform-mariadb-cluster

This Terraform module creates infrastructure for a MariaDB Cluster along with a Bastion Host. After deployment of the infrastructure the Bastion Host should be used to install deploy the remaining objects to MariaDB.

# module structure

* ansible/ - Contains Ansible resources for deployment of MariaDB on the infrastructure.
* examples/ - Contains examples for using the module.
* modules/ - Contains nested modules
  * terraform-mariadb-cloudwatch - Cloudwatch Alarms for the MariaDB Cluster Instances.
  * terraform-dba-bastion - Bastion host for the MariaDB Cluster.
  * TODO
* main.tf
* outputs.tf
* variables.tf
