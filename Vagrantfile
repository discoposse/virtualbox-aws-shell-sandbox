# -*- mode: ruby -*-
# vi: set ft=ruby :

VAGRANTFILE_API_VERSION = "2"
ENV['VAGRANT_DEFAULT_PROVIDER'] = 'virtualbox'

Vagrant.configure(VAGRANTFILE_API_VERSION) do |config|
  config.vm.define "awssandbox" do |awssandbox|
    awssandbox.vm.hostname = "awssandbox"
    awssandbox.vm.box = "trusty-server"
    awssandbox.vm.box_url = "https://oss-binaries.phusionpassenger.com/vagrant/boxes/latest/ubuntu-14.04-amd64-vbox.box"
    awssandbox.vm.provision :shell, :path => "build.sh"
  end
end