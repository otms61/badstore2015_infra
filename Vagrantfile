# -*- mode: ruby -*-
Vagrant.configure(2) do |config|
  config.vm.box = "chef/centos-6.5"
  config.vm.network "private_network", ip: "192.168.40.10"
  config.vm.provision :ansible do |ansible|
    ansible.playbook = "provision_vagrant.yml"
    ansible.inventory_path = "hosts"
    ansible.limit = "all"
  end
end
