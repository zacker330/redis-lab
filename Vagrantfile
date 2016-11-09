# -*- mode: ruby -*-
# vi: set ft=ruby :

# All Vagrant configuration is done below. The "2" in Vagrant.configure
# configures the configuration version (we support older styles for
# backwards compatibility). Please don't change it unless you know what
# you're doing.
Vagrant.configure(2) do |config|

  machine_box = "bento/ubuntu-16.04"
  machine_box_url = "https://atlas.hashicorp.com/bento/boxes/ubuntu-16.04/versions/2.3.0/providers/virtualbox.box"

  config.vm.define "node-redis-1" do |machine|
    machine.vm.box = machine_box
    machine.vm.box_url = machine_box_url
    machine.vm.hostname = "node-redis-1"
    machine.vm.network "private_network", ip: "192.168.8.11"
    machine.vm.provider "virtualbox" do |node|
        node.name = "node-redis-1"
        node.memory = 1024
        node.cpus = 2
    end
   end

   config.vm.define "node-redis-2" do |machine|
     machine.vm.box = machine_box
     #machine.vm.box_url = machine_box_url
     machine.vm.hostname = "node-redis-2"
     machine.vm.network "private_network", ip: "192.168.8.12"
     machine.vm.provider "virtualbox" do |node|
         node.name = "node-redis-2"
         node.memory = 1024
         node.cpus = 2
     end
    end

end
