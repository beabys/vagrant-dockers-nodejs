# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|
  config.vm.box = "vcraescu/ubuntu-16.04-docker"
  config.vm.hostname = 'node.dev'
  config.vm.provider "virtualbox" do |vb|
      vb.gui = false
      vb.name = "node-esqueleton.dev"
  end
  config.vm.network "private_network", ip: "192.168.56.105"
  config.vm.network "forwarded_port", guest: 80, host: 80
  config.vm.synced_folder ".", "/var/www"
  config.vm.synced_folder ".", "/vagrant", disabled: "true"
  config.vm.provision :docker_compose, rebuild: true, run: "always", yml: "/var/www/docker/docker-compose.yml"
end
