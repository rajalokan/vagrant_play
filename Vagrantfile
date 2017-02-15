# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|
  config.vm.box = "ubuntu/xenial64"
  config.vm.hostname = "playbox"
  config.vm.provision "ansible_local" do |ansible|
    ansible.playbook = "bootstrap.yml"
	ansible.galaxy_role_file = "requirements.yml"
	ansible.galaxy_roles_path = "/tmp/roles/"
  end

end
