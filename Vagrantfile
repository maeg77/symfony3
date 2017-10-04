Vagrant.configure("2") do |config|
  config.vm.box = "ubuntu/trusty64"

  config.vm.synced_folder ".", "/opt/app"

  config.vm.provision :ansible do |ansible|
      ansible.playbook = "provisioning/playbook.yml"
    end
end
