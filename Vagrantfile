
Vagrant.configure("2") do |config|
  config.vm.box = "ubuntu/focal64"
  config.vm.network "forwarded_port", guest: 80, host: 8090
  config.vm.network "public_network"
  config.vm.synced_folder "site/", "/var/www/html"
  config.vm.provision "ansible" do |ansible|
    ansible.playbook = "playbook.yml"

  
  end
end
