# -*- mode: ruby -*-
# vi: set ft=ruby :

# All Vagrant configuration is done below. The "2" in Vagrant.configure
# configures the configuration version (we support older styles for
# backwards compatibility). Please don't change it unless you know what
# you're doing.
Vagrant.configure(2) do |config|
  config.vm.define "snort" do |snort|
    snort.vm.box = "mrlesmithjr/trusty64"
    snort.vm.hostname = "snort"

    snort.vm.network :private_network, ip: "192.168.202.201"
    
    snort.vm.provider "virtualbox" do |vb|
      vb.memory = "1024"
    end
  end
  config.vm.provision :shell, path: "provision.sh"
end
