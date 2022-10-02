Vagrant.configure("2") do |config|
  # Every Vagrant development environment requires a box. You can search for
  # boxes at https://vagrantcloud.com/search.
  config.vm.define "server" do |server|
   server.vm.box = "geerlingguy/centos7"
   server.vm.hostname = "server"
   config.vm.network "public_network", bridge: "enp8s0", :mac => "5CA1AB1E0001"
   config.vm.provision "shell", inline: <<-SHELL
   sed -i 's/PasswordAuthentication no/PasswordAuthentication yes/g' /etc/ssh/sshd_config    
   systemctl restart sshd.service
SHELL
  end
 end
