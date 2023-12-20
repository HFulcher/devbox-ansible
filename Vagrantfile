# -*- mode: ruby -*-
# vi: set ft=ruby :
Vagrant.configure("2") do |config|
  config.vm.box = "d3r/bookworm"
  config.vm.box_version = "1.0"

  config.vm.provider :parallels do |p|
    p.name = "devbox"
  end

  config.vm.provision "ansible" do |a|
    a.verbose = "v"
    a.playbook = "run.yml"
  end
end

