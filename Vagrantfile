Vagrant.configure("2") do |config|
  MONGOS_HOSTS=3
  (1..MONGOS_HOSTS).each do |mongos|
    node_name = "mongos#{mongos}"
    config.vm.define node_name do |mongos_node|
      mongos_node.vm.box = "centos/7"
      mongos_node.vm.network "private_network", ip: "192.168.43.#{100 + mongos}"
      mongos_node.vm.hostname = node_name
      mongos_node.vm.provision :shell, path: "bash/bootstrap_avahi.sh", run: "always"
      mongos_node.vm.provision :shell, path: "bash/install_ansible.sh", run: "always"
      mongos_node.vm.synced_folder "MongoDBCluster/", "/home/vagrant/ansible"
    end
  end
  MONGOD_HOSTS=6
  (1..MONGOD_HOSTS).each do |mongod|
    node_name = "mongod#{mongod}"
    config.vm.define node_name do |mongod_node|
      mongod_node.vm.box = "centos/7"
      mongod_node.vm.network "private_network", ip: "192.168.43.#{200 + mongod}"
      mongod_node.vm.hostname = "mongod1"
      mongod_node.vm.provision :shell, path: "bash/bootstrap_avahi.sh", run: "always"
      if mongod_node == MONGOD_HOSTS
        mongod_node.vm.provision :ansible do |ansible|
        ansible.limit = "all" # Connect to all machines
        ansible.playbook = "mongodb.yaml"
      end
    end
  end
end
end
