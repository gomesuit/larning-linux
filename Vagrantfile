# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure('2') do |config|
  config.vm.box = 'bento/ubuntu-16.04'
  config.ssh.forward_agent = true

  config.vm.define :server do |host|
    host.vm.hostname = 'server'
    host.vm.network :private_network, ip: '192.168.33.10'
    host.vm.provision :shell, path: 'provision.sh'
  end
end
