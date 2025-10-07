Vagrant.configure("2") do |config|
  config.vm.box = "hashicorp/bionic64"
  # config.vm.box_check_update = false
  # guest é a porta do serviço e host é a porta de acesso via local
  config.vm.network "forwarded_port", guest: 80, host: 8080

  config.vm.network "private_network", ip: "10.0.1.100"

  # config.vm.synced_folder "../data", "/vagrant_data"

  config.vm.synced_folder "site/", "/var/www/html"

  # config.vm.provider "virtualbox" do |vb|
  #   vb.memory = "1024"
  # end
  config.vm.provision "shell", path: "script.sh"

end
