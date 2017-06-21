Vagrant.configure("2") do |config|

  config.vm.define "gw01" do |gw01|
    gw01.vm.box = "ubuntu/trusty64"
    gw01.vm.hostname = "gw01"
    gw01.vm.network "private_network", ip: "192.168.0.100", virtualbox__intnet: true
    gw01.vm.network "public_network", use_dhcp_assigned_default_route: true
  end

  config.vm.define "gw02" do |gw02|
    gw02.vm.box = "ubuntu/trusty64"
    gw02.vm.hostname = "gw02"
    gw02.vm.network "private_network", ip: "192.168.0.200", virtualbox__intnet: true
    gw02.vm.network "public_network", use_dhcp_assigned_default_route: true
  end

  config.vm.provider "virtualbox" do |v|
    v.memory = 512
    v.cpus = 1
  end

end
