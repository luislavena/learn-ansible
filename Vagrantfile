Vagrant.configure("2") do |config|
  # Ubuntu 13.04 box
  # See vms/README.md
  config.vm.box = "raring64-packer"

  config.vm.define "aio-stage" do |box|
    # RAM: 1.5GB
    box.vm.provider "virtualbox" do |vb|
      vb.customize ["modifyvm", :id, "--memory", "1536"]
    end

    # FIXME: setup two interfaces (public + private)
    # box.vm.network "public_network",  bridge: "en0: Wi-Fi (AirPort)"
    box.vm.network "private_network", ip: "192.168.33.100"

    # provision with Ansible
    box.vm.provision "ansible" do |ansible|
      ansible.playbook       = "playbook.yml"
      ansible.inventory_path = "inventories/aio-stage-vagrant/hosts"
      ansible.verbose        = true
    end
  end
end
