Vagrant.configure("2") do |config|
    config.vm.box = "ubuntu/xenial64"

    config.vm.define 'ubuntu' do |node|
        node.vm.hostname = 'ubuntu.local'
        node.vm.provision "ansible" do |ansible|
            ansible.playbook = "main.yml"
        end
    end
end