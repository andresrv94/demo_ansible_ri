
Vagrant.configure("2") do |config|

    config.vm.box = "ubuntu/focal64"

    config.vm.define "instancia1" do |instancia1|
        instancia1.vm.network :private_network, ip: "192.168.56.253"
        

        instancia1.vm.provider "virtualbox" do |vb|
            vb.gui = false
            vb.memory = "1024"
            vb.cpus = "1"
        end
    end

    config.vm.define "instancia2" do |instancia2|
        instancia2.vm.network :private_network, ip: "192.168.56.254"
        

        instancia2.vm.provider "virtualbox" do |vb|
            vb.gui = false
            vb.memory = "1024"
            vb.cpus = "1"
        end
    end


end
