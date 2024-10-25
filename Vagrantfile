Vagrant.configure("2") do |config|
  
  config.vm.box = "debian/bookworm64"

  config.vm.provision "shell", inline: <<-SHELL
    apt-get update
    apt-get install -y bind9
  SHELL

  config.vm.define "venus" do |venus|
    venus.vm.network "private_network", ip: "192.168.57.102"
    venus.vm.provision "shell", inline: <<-SHELL
    sudo su
    cp -v /vagrant/named.conf.local.venus /etc/bind/named.conf.local
    systemctl restart bind9
    SHELL
  end

  config.vm.define "tierra" do |tierra|
    tierra.vm.network "private_network", ip: "192.168.57.103"
    tierra.vm.provision "shell", inline: <<-SHELL
    sudo su
    cp -v /vagrant/named /etc/default
    cp -v /vagrant/named.conf.local /etc/bind/named.conf.local
    cp -v /vagrant/ex1.diego /etc/bind/named.conf.options
    cp -v /vagrant/db.sistma.test /etc/bind/db.sistma.test
    cp -v /vagrant/zona.inversa /etc/bind/db.192

    systemctl restart bind9

  end
end