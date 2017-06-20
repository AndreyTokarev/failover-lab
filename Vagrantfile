Vagrant.configure("2") do |config|
  config.vm.box = "ubuntu/trusty64"

  config.vm.define "gw01" do |gw01|
    gw01.vm.box = "gw01"
    gw01.vm.network "private_network", ip: "192.168.0.100"
  end

  config.vm.define "gw02" do |gw02|
    gw02.vm.box = "gw02"
    gw02.vm.network "private_network", ip: "192.168.50.200"
end
end
