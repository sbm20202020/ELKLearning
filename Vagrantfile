Vagrant.configure("2") do |config|
  config.vm.define "elasticsearch" do |elasticsearch|
    elasticsearch.vm.box = "aspyatkin/ubuntu-20.04-server"
    elasticsearch.vm.network "public_network", bridge: "wlp2s0"
    elasticsearch.vm.network "forwarded_port", guest: 9200, host: 9200
    elasticsearch.vm.hostname = "elasticsearch"
    elasticsearch.vm.provider "virtualbox" do |vb|
      vb.name = "elasticsearch"
      vb.memory = "4096"
      vb.cpus = "2"
    end
  
    # Disk size of the VM
    elasticsearch.disksize.size = '20GB'
  end
end
