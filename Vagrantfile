Vagrant.configure("2") do |config|
  config.vm.box = "hashicorp/bionic64"
  # config.vm.box_check_update = false
  # guest é a porta do serviço e host é a porta de acesso via local
    config.vm.network "forwarded_port", guest: 80, host: 8080

<<<<<<< HEAD
  config.vm.network "private_network", ip: "10.0.1.100"
=======
  # config.vm.network "forwarded_port", guest: 80, host: 8080, host_ip: "127.0.0.1"

  # config.vm.network "private_network", ip: "192.168.33.10"

    config.vm.network "public_network"
>>>>>>> a3d52f717c295292a194ff1a93bedfb673d3e93a

  # config.vm.synced_folder "../data", "/vagrant_data"

  config.vm.synced_folder "site/", "/var/www/html"

  # config.vm.provider "virtualbox" do |vb|
  #   vb.memory = "1024"
  # end
  config.vm.provision "shell", path: "script.sh"

end
