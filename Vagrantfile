Vagrant.configure("2") do |config|
  config.vm.define "jenkins" do |node|
    node.vm.box = "ubuntu/bionic64"
    node.vm.network "public_network", ip: "192.168.1.76"
  end

  config.vm.provision "ansible" do |ansible|
    ansible.playbook = "ansible-jenkins.yml"
  end
end
