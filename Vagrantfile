Vagrant.configure("2") do |config|
    config.vm.box = "ubuntu/bionic64"
  
    # Servidor 1
    config.vm.define "server1" do |server1|
      server1.vm.hostname = "server1"
      server1.vm.network "private_network", ip: "192.168.56.101"
      server1.vm.network "forwarded_port", guest: 22, host: 2222
      server1.vm.provider "virtualbox" do |vb|
        vb.memory = "256"
        vb.cpus = 1
      end
    end
  
    # Servidor 2
    config.vm.define "server2" do |server2|
      server2.vm.hostname = "server2"
      server2.vm.network "private_network", ip: "192.168.56.102"
      server2.vm.network "forwarded_port", guest: 22, host: 2223
      server2.vm.provider "virtualbox" do |vb|
        vb.memory = "256"
        vb.cpus = 1
      end
    end
  
    # Servidor 3
    config.vm.define "server3" do |server3|
      server3.vm.hostname = "server3"
      server3.vm.network "private_network", ip: "192.168.56.103"
      server3.vm.network "forwarded_port", guest: 22, host: 2224
      server3.vm.provider "virtualbox" do |vb|
        vb.memory = "256"
        vb.cpus = 1
      end
    end
  end

  