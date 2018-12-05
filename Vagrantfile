# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure('2') do |config|
  config.vm.box = 'Microsoft/EdgeOnWindows10'

  config.vm.network 'public_network', bridge: 'enp0s31f6', nic_type: '82540EM'
  config.vm.network 'public_network', bridge: 'wlp3s0', nic_type: '82540EM'

  config.vm.provider 'virtualbox' do |vb|
    vb.gui = true
    vb.memory = '2024'
    vb.cpus = 2
    vb.customize ['modifyvm', :id, '--vram', '64']
  end
end
