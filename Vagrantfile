Vagrant.configure("2") do |config|

  config.vm.define "mongos1" do |mongos1|
    mongos1.vm.box = "centos/7"
    mongos1.vm.network "private_network", ip: "192.168.43.100"
    mongos1.vm.hostname = "mongos1"
    mongos1.vm.provision :shell, path: "bash/bootstrap_avahi.sh", run: "always"
    mongos1.vm.provision :shell, path: "bash/install_ansible.sh", run: "always"
  end
  
  config.vm.define "mongos2" do |mongos2|
    mongos2.vm.box = "centos/7"
    mongos2.vm.network "private_network", ip: "192.168.43.101"
    mongos2.vm.hostname = "mongos2"
    mongos2.vm.provision :shell, path: "bash/bootstrap_avahi.sh", run: "always"
    mongos2.vm.provision :shell, path: "bash/install_ansible.sh", run: "always"
  end
  
  config.vm.define "mongos3" do |mongos3|
    mongos3.vm.box = "centos/7"
    mongos3.vm.network "private_network", ip: "192.168.43.102"
    mongos3.vm.hostname = "mongos3"
    mongos3.vm.provision :shell, path: "bash/bootstrap_avahi.sh", run: "always"
    mongos3.vm.provision :shell, path: "bash/install_ansible.sh", run: "always"
  end  

  config.vm.define "mongod1" do |mongod1|
    mongod1.vm.box = "centos/7"
    mongod1.vm.network "private_network", ip: "192.168.43.103"
    mongod1.vm.hostname = "mongod1"
    mongod1.vm.provision :shell, path: "bash/bootstrap_avahi.sh", run: "always"
  end
  
  config.vm.define "mongod2" do |mongod2|
    mongod2.vm.box = "centos/7"
    mongod2.vm.network "private_network", ip: "192.168.43.104"
    mongod2.vm.hostname = "mongod2"
    mongod2.vm.provision :shell, path: "bash/bootstrap_avahi.sh", run: "always"
  end  
 
  config.vm.define "mongod3" do |mongod3|
    mongod3.vm.box = "centos/7"
    mongod3.vm.network "private_network", ip: "192.168.43.105"
    mongod3.vm.hostname = "mongod3"
    mongod3.vm.provision :shell, path: "bash/bootstrap_avahi.sh", run: "always"
  end  
 
   config.vm.define "mongod4" do |mongod4|
    mongod4.vm.box = "centos/7"
    mongod4.vm.network "private_network", ip: "192.168.43.106"
    mongod4.vm.hostname = "mongod4"
    mongod4.vm.provision :shell, path: "bash/bootstrap_avahi.sh", run: "always"
  end
  
  config.vm.define "mongod5" do |mongod5|
    mongod5.vm.box = "centos/7"
    mongod5.vm.network "private_network", ip: "192.168.43.107"
    mongod5.vm.hostname = "mongod5"    
    mongod5.vm.provision :shell, path: "bash/bootstrap_avahi.sh", run: "always"
  end  
 
  config.vm.define "mongod6" do |mongod6|
    mongod6.vm.box = "centos/7"
    mongod6.vm.network "private_network", ip: "192.168.43.108"
    mongod6.vm.hostname = "mongod6"    
    mongod6.vm.provision :shell, path: "bash/bootstrap_avahi.sh", run: "always"
  end  
  
end

