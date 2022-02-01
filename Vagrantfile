Vagrant.configure("2") do |config|

  config.vm.define "proxy" do |proxy|
    proxy.vm.box = "centos/7"
    proxy.vm.hostname = "machine1"
  
    proxy.vm.provider :virtualbox do |v|
      v.memory = 2048
      v.cpus = 2
    end
  end

  config.vm.define "app" do |app|
    app.vm.box = "ubuntu/trusty64"
    app.vm.hostname = "machine2"

    app.vm.provider :virtualbox do |v|
      v.memory = 2048
      v.cpus = 2

    end
  end

end