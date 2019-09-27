Vagrant.configure("2") do |config|
config.vm.box = "ubuntu/trusty64"
 config.vm.define "ubuntu" do |ubuntu|
  ubuntu.vm.network "private_network", ip: "172.20.20.10"
 end

 config.vm.define "centos" do |centos|
  centos.vm.network "private_network", ip: "172.20.20.11"
 end  
#config.vm.network "forwarded_port", guest: 80, host: 8080
#config.vm.network "forwarded_port", guest: 80, host: 8080, host_ip: "127.0.0.1"

#config.vm.network "private_network", ip: "192.168.33.10"

#config.vm.synced_folder "../data", "/vagrant_data"
config.vm.provision "shell", inline: <<-SHELL
     apt-get update
     apt-get install -y apache2
   SHELL
end
