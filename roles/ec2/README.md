ec2
=========

This Role launch ec2 instances on aws with 1 master and 3 slave by using instance type t2.micro

Requirements
------------

Any pre-requisites that may not be covered by Ansible itself or the role should be mentioned here. For instance, if the role uses the EC2 module, it may be a good idea to mention in this section that the boto package is required.

Role Variables
--------------
* key: instance key Name
* aws_instance_type: family type
* count_master: no. of master(1)
* count_slave: no. of slave(3), you can change.
* ami_id: AMI_ID
* subnet_id: Subnet ID
* aws_region: Region
* security_group_id: SG's

Dependencies
------------

A list of other roles hosted on Galaxy should go here, plus any details in regards to parameters that may need to be set for other roles, or variables that are used from other roles.

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - { role: username.rolename, x: 42 }
