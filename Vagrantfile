Vagrant.configure("2") do |config|
  config.vm.box = "centos/7"

  config.vm.provider "vmware_fusion" do |vmware|
    vmware.gui = false
    vmware.vmx["vhv.enable"] = "TRUE"
  end

  config.vm.provision "ansible_local" do |ansible|
    ansible.install_mode = "pip"
    ansible.playbook =  "provision/ansible/site.yml"
  end
end
