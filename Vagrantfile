# -*k mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|
    config.vm.box = "bento/ubuntu-22.04"
#        
    config.vm.define "master" do |master|
            master.vm.box = "bento/ubuntu-22.04"
            master.vm.hostname="master"
            master.vm.provider "virtualbox" do |vb|
            vb.memory = 4096
            vb.cpus = 2
            end
            master.vm.network :private_network,
                            :ip => '192.168.1.10'

    end

config.vm.define "worker1" do |worker1|
         worker1.vm.box = "bento/ubuntu-22.04"
         worker1.vm.hostname="worker1"
         worker1.vm.provider "virtualbox" do |vb|
            vb.memory = 2048
            vb.cpus = 2
            end
         worker1.vm.network :private_network, :ip => '192.168.1.11'
end 
config.vm.define "worker2" do |worker2|
    worker2.vm.box = "bento/ubuntu-22.04"
    worker2.vm.hostname="worker2"
    worker2.vm.provider "virtualbox" do |vb|
       vb.memory = 2048
       vb.cpus = 2
       end
    worker2.vm.network :private_network, :ip => '192.168.1.12'
end 

end