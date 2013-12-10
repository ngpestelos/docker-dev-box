# -*- mode: ruby -*-
# vi: set ft=ruby :

# Vagrantfile API/syntax version. Don't touch unless you know what you're doing!
VAGRANTFILE_API_VERSION = "2"

VM_BOX = "saucy64"
VM_BOX_URL = "https://dl.dropboxusercontent.com/u/6154794/Vagrant/saucy64.box"

Vagrant.configure(VAGRANTFILE_API_VERSION) do |config|
  config.vm.box = VM_BOX
  config.vm.box_url = VM_BOX_URL

  config.vm.provision :docker do |docker|
    docker.version = '0.7.0'
    docker.pull_images 'ubuntu'
  end
end
