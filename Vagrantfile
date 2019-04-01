# -*- mode: ruby -*-
# vi: set ft=ruby :
VAGRANTFILE_API_VERSION = "2"
Vagrant.configure(VAGRANTFILE_API_VERSION) do |config|
config.ssh.insert_key = false
#config.vm.provider :virtualbox do |vb|
#vb.customize ["modifyvm", :id, "--memory", "256"]
#end
# nagios master 
config.vm.define "nagios" do |nagios|
nagios.vm.hostname = "nagios.dev"
nagios.vm.box = "geerlingguy/centos7"
nagios.vm.network :private_network, ip: "192.168.60.4"
end
# node 1
config.vm.define "node1" do |node1|
node1.vm.hostname = "node1.dev"
node1.vm.box = "geerlingguy/centos7"
node1.vm.network :private_network, ip: "192.168.60.5"
end
# node 2 
config.vm.define "node2" do |node2|
node2.vm.hostname = "node2.dev"
node2.vm.box = "geerlingguy/centos7"
node2.vm.network :private_network, ip: "192.168.60.6"
end
# node 3 
config.vm.define "node3" do |node3|
node3.vm.hostname = "node3.dev"
node3.vm.box = "geerlingguy/centos7"
node3.vm.network :private_network, ip: "192.168.60.7"
end
end
