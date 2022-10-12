guest_ip  = "192.168.56.4"

ENV['VAGRANT_DEFAULT_PROVIDER'] = 'virtualbox'
Vagrant.configure("2") do |config|
  config.vm.box = "generic/rhel7"
  config.vm.network "private_network", ip: guest_ip
  config.vm.provision "shell", path: "provision.sh"
  config.vm.synced_folder "C:\\Dev\\Treinamentos\\Vagrantfile\\rhel79-lab2", "/vagrant"
  #config.vm.provision "ansible_local" do |ansible|
    #ansible.playbook       = "playbook.yml"
    #ansible.install_mode = "pip"    
    #ansible.pip_install_cmd = "sudo yum install -y python3-distutils && curl https://bootstrap.pypa.io/get-pip.py | sudo python3"
    #ansible.galaxy_command = "sudo ansible-galaxy install -r /vagrant/collections/requirements.yml"
  #end
end
