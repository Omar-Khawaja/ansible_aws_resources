This Ansible playbook provisions EC2 instances and dynamically creates
a host group consisting of these new nodes. Using in-memory inventory,
Ansible can immediately configure these new resources in subsequent plays
using the same playbook.

This particular playbook will add the newly provisioned EC2 instances to
the host group labeled "newly_created" and then install httpd on each of them. 

Please note: Authentication wtih AWS-related modules requires an AWS access
key and secret key. For more information on this subject, refer to Ansible's
documentation: http://docs.ansible.com/ansible/guide_aws.html


