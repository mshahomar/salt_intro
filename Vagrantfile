
Vagrant.configure("2") do |config|
  config.vm.define "master" do |subconfig|
    subconfig.vm.box = "bento/centos-7.5"
    subconfig.vm.hostname = "salt-master"
    subconfig.vm.network "private_network", ip: "10.0.2.100",
      virtualbox__intnet: true
  end

  config.vm.define "minion1" do |subconfig|
    subconfig.vm.box = "bento/ubuntu-18.04"
    subconfig.vm.hostname = "jerry"
    subconfig.vm.network "private_network", ip: "10.0.2.101",
      virtualbox__intnet: true
  end

  config.vm.define "minion2" do |subconfig|
    subconfig.vm.box = "bento/ubuntu-18.04"
    subconfig.vm.hostname = "stuart"
    subconfig.vm.network "private_network", ip: "10.0.2.102",
      virtualbox__intnet: true
  end

end
