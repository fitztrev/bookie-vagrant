# -*- mode: ruby -*-
# vi: set ft=ruby :

BOOKIE_REPO = "-b non-interactive-install https://github.com/fitztrev/Bookie.git"

VAGRANTFILE_API_VERSION = "2"

Vagrant.configure(VAGRANTFILE_API_VERSION) do |config|
  config.vm.box     = "precise64"
  config.vm.box_url = "http://files.vagrantup.com/precise64.box"

  ## Setup port forwarding
  config.vm.network :forwarded_port, guest: 6543, host: 6543

  ## Provision
  config.vm.provision "shell", inline: "sudo apt-get update"
  config.vm.provision "shell", inline: "sudo apt-get install -y build-essential git"
  config.vm.provision "shell", inline: "[ ! -d /vagrant/Bookie ] && git clone #{BOOKIE_REPO} /vagrant/Bookie || echo 'Repo exists. Skipping.'"
  config.vm.provision "shell", inline: "cd /vagrant/Bookie && NONINTERACTIVE=true make sysdeps && make install && make run"
end
