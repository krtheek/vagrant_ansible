# -*- mode: ruby -*-
# vi: set ft=ruby :
Vagrant.configure(2) do |config|

config.vm.define "ansible" do |ansible|
	ansible.vm.box = "centos/7"
	ansible.vm.network "private_network", ip: "192.168.56.220"
	ansible.vm.hostname = "controller"
	config.vm.provider "virtualbox" do |v|
		v.memory = 2048
		v.cpus = 2
	end
end

config.vm.define "node1" do |node1|
node1.vm.box = "centos/7"
node1.vm.network "private_network", ip: "192.168.56.221"
node1.vm.hostname = "node1"
end


config.vm.define "node2" do |node2|
node2.vm.box = "centos/7"
node2.vm.network "private_network", ip: "192.168.56.222"
node2.vm.hostname = "node2"
end


config.vm.define "node3" do |node3|
node3.vm.box = "ubuntu/trusty64"
node3.vm.network "private_network", ip: "192.168.56.223"
node3.vm.hostname = "node3"
end

end


