# -*- mode: ruby -*-
# vi: set ft=ruby :
#
# This file gets used for testing the deployment with internal CI

Vagrant.configure("2") do |config|
  config.vm.provider :libvirt do |libvirt, override|
    libvirt.memory = 2048
  end
  config.vm.box = "windows-10"
  config.vm.provision "ansible" do |ansible|
    ansible.playbook = "site.yml"
    ansible.extra_vars = {
        ansible_winrm_server_cert_validation: "ignore",
        ansible_winrm_transport: "ntlm",
    }
  end
end
