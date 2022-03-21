Vagrant.configure("2") do |config|
  config.vm.box = "hashicorp/bionic64"

  config.vm.provider "virtualbox" do |vb|
    vb.name = "mydb"
    vb.memory = "1024"
    vb.cpus = 1
  end

  config.vm.hostname = "mydb"

  config.vm.provision "shell", path: "postgres.sh"
end
