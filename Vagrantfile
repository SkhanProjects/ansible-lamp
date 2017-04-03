# -*- mode: ruby -*-
# vi: set ft=ruby :


# you're doing.
Vagrant.configure("2") do |config|
 
  config.vm.box = "ubuntu/trusty64"

  #config.vm.network "forwarded_port",  guest: 80 , host: 8080
  config.vm.network "private_network", ip: "192.168.33.12"

  config.vm.synced_folder ".", "/var/www"

  config.vm.provision :ansible do |ansible|
  ansible.playbook = "mainpl.yml"


  end

end
