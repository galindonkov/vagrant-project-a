Vagrant.configure("2") do |config|
  config.vm.box = "galindonkov/xenial64"
  config.vm.box_version = "0.1"
  config.vm.hostname = "bananas3"
  config.vm.network "private_network", ip: "192.168.56.56"
  config.vm.provision "shell", path: "scripts/provision.sh"
  config.vm.network "forwarded_port", guest: 80, host: 8080,  auto_correct: "true"
end
