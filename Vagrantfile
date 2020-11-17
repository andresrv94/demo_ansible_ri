Vagrant.configure("2") do |config|

    config.vm.box = "ubuntu/focal64"
    config.vm.define "instancia1" do |instancia1|
        instancia1.vm.network :private_network, ip: "192.168.56.253"
        config.ssh.insert_key = false
        config.vm.provision "file", source: "~/.ssh/id_rsa.pub", destination: "~/.ssh/authorized_keys" 
        config.ssh.private_key_path = ['~/.vagrant.d/insecure_private_key','~/.ssh/id_rsa']
        instancia1.vm.provider "virtualbox" do |vb|
            vb.gui = false
            vb.memory = "1024"
            vb.cpus = "1"
        end
    end

    config.vm.define "instancia2" do |instancia2|
        instancia2.vm.network :private_network, ip: "192.168.56.254"
        config.ssh.insert_key = false
        config.vm.provision "file", source: "~/.ssh/id_rsa.pub", destination: "~/.ssh/authorized_keys" 
        config.ssh.private_key_path = ['~/.vagrant.d/insecure_private_key','~/.ssh/id_rsa']
        instancia2.vm.provider "virtualbox" do |vb|
            vb.gui = false
            vb.memory = "1024"
            vb.cpus = "1"
        end
    end


end
