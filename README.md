# MongoDBCluster
A Vagrant and Ansible project to deploy a test MongoDB Cluster with sharding.

A total of 9 VMs will be created by vagrant.

# To get started (from project root)
vagrant up;

# Check VM status
vagrant status;

	Current machine states:

	mongos1                   running (virtualbox)
	mongos2                   running (virtualbox)
	mongos3                   running (virtualbox)
	mongod1                   running (virtualbox)
	mongod2                   running (virtualbox)
	mongod3                   running (virtualbox)
	mongod4                   running (virtualbox)
	mongod5                   running (virtualbox)
	mongod6                   running (virtualbox)
	
	This environment represents multiple VMs. The VMs are all listed
	above with their current state. For more information about a specific
	VM, run `vagrant status NAME`.

# Ansible Playbook

# Role created with;
ansible-galaxy init MongoDBCluster;

Archived. see here for the future: https://github.com/rhysmeister/AutomatingMongoDBWithAnsible
