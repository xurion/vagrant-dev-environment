Vagrant.configure("2") do |config|

  config.vm.hostname = "lamp"

  config.vm.network :private_network, ip: "192.168.50.4"

  # Our packaged basebox should be based of Ubuntu 12.04 32bit.

  config.vm.box = "precise32"
  config.vm.box_url = "http://files.vagrantup.com/precise32.box"

  # Provision the box with a shell script.

  config.vm.provision :shell, :path => "provision/provision.sh"

  config.vm.synced_folder "~/Sites/", "/home/vagrant/Sites"

end
