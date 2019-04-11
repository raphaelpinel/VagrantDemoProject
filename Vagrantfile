Vagrant.configure("2") do |config|
  config.vm.box = "ubuntu/xenial64"
  config.vm.provision :shell, path: "bootstrap.sh"
  config.vm.network :forwarded_port, guest: 8080, host: 8080
  config.vm.network :forwarded_port, guest: 8081, host: 8081
  config.vm.network :forwarded_port, guest: 8082, host: 8082
  config.vm.network :forwarded_port, guest: 8083, host: 8083
  config.vm.network :forwarded_port, guest: 3000, host: 3000
  config.vm.network :forwarded_port, guest: 5000, host: 5000
  config.vm.hostname = "Jenkins"
  config.vm.provider "virtualbox" do |v|
    v.memory = 2048
    v.cpus = 2
  end
end