##  Magento Community Edition

- Requires Ansible 1.2 or newer
- Expects CentOS/RHEL 6.x hosts

These playbooks deploy a very basic implementation of the open source Magento Community Edition eCommerce solution,
version 1.7. To use them, first edit the "hosts" inventory file to contain the
hostnames of the machines on which you want Magento deployed, and edit the 
group_vars/magento-servers file to set any Magento installation parameters you need.

Then run the playbook, like this:

	ansible-playbook -i hosts site.yml

When the playbook run completes, you should be able to see the Magento running on the ports you chose, on the target machines.

This is a very simple playbook and could serve as a starting point for more
complex Magento implementations. 

### Ideas for Improvement

Here are some ideas for ways that these playbooks could be extended:

- Extend to work with other versions of Magento
- Extend to work with Magento Enterprise Edition

We would love to see contributions and improvements, so please fork this
repository on GitHub and send us your changes via pull requests.
