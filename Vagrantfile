# -*- mode: ruby -*-
# vi: set ft=ruby :

# Vagrantfile API/syntax version. Don't touch unless you know what you're doing!
VAGRANTFILE_API_VERSION = "2"

Vagrant.configure(VAGRANTFILE_API_VERSION) do |config|
  config.vm.define "ubuntu-jammy64" do |m|
    m.vm.box = "ubuntu/jammy64"
    m.vm.provision "ansible" do |ansible|
      ansible.playbook = "site.yml"
      ansible.limit = 'all'
    end
  end
end
