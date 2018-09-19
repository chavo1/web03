Vagrant.configure("2") do |config|
  config.vm.box = "chavo1/oracle75-nginx"
  config.vm.hostname = "bananas3"
  config.vm.network "private_network", ip: "192.168.56.56"
  config.vm.network "forwarded_port", guest: 80, host: 8080, auto_correct: "true"
  config.vm.provision "shell", path: "scripts/provision.sh"

end
