# Vagrantfile API/syntax version. Don't touch unless you know what you're doing!
VAGRANTFILE_API_VERSION = "2"

Vagrant.configure(VAGRANTFILE_API_VERSION) do |config|
  config.vm.box = "hashicorp/precise64"
  config.vm.network :forwarded_port, host: 4567, guest: 80
  config.vm.provision :shell, :path => "bootstrap.sh"
end
