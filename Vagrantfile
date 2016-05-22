# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure(2) do |config|

  config.vm.box = "box-cutter/ubuntu1404-desktop"

  config.vm.provision "ansible" do |ansible|
    ansible.playbook = "playbook.yml"
		ansible.verbose = 'vv'
  end

  config.vm.synced_folder "dotfiles/","/home/vagrant/dotfiles/"
end
