Vagrant.configure("2") do |config|

  # configures vm settings
  config.vm.box = "ubuntu/xenial64"
  config.vm.network "private_network", ip:"192.168.1.110"

  # provision the VM to have nginx
  config.vm.provision "shell", path: "provision.sh"

  # put the app folder from local machine to the VM
  config.vm.synced_folder "app", "/home/vagrant/app/app"

end
