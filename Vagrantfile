
# Arquivo de configuração do vagrant + ansible Rivendel Tecnologia
 Vagrant.configure(2) do |config|

    config.vm.box = "centos/7"
    config.vm.network "private_network", ip: "192.168.33.10"
    #config.vm.network "forwarded_port", guest: 80, host: 8080

    # Disable the new default behavior introduced in Vagrant 1.7, to
    # ensure that all Vagrant machines will use the same SSH key pair.
    # See https://github.com/mitchellh/vagrant/issues/5005
    #  config.ssh.insert_key = false
      config.vm.provision "ansible" do |ansible|
      ansible.playbook = "playbook.yml"
    end
end
