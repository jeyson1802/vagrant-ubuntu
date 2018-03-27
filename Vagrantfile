# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure(2) do |config|
	config.vm.box = "ubuntu/trusty64"
	
		config.vm.define :node1 do |node1_config|
			node1_config.vm.host_name = "node1"
			node1_config.vm.network "private_network", ip:"10.230.168.100"
			node1_config.vm.provider :virtualbox do |vb|
				vb.customize ["modifyvm", :id, "--memory", "1024"]
				vb.customize ["modifyvm", :id, "--cpus", "1"]
			end
		end
		
		config.vm.define :node2 do |node2_config|
			node2_config.vm.host_name = "node2"
			node2_config.vm.network "private_network", ip:"10.230.168.100"
			node2_config.vm.provider :virtualbox do |vb|
				vb.customize ["modifyvm", :id, "--memory", "1024"]
				vb.customize ["modifyvm", :id, "--cpus", "1"]
			end
		end
	
end