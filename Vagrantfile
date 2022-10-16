Vagrant.configure("2") do |config|
  
    config.vm.define "scriptbox" do |scriptbox|
        scriptbox.vm.box = "spox/ubuntu-arm"
        scriptbox.vm.hostname = "scriptbox"
        scriptbox.vm.network "private_network", ip: "192.168.10.2"
    end
  
    config.vm.define "web01" do |web01|
      web01.vm.box = "jacobw/fedora35-arm64"
      web01.vm.hostname = "web01"
      web01.vm.network "private_network", ip: "192.168.10.3"
    end

    config.vm.define "web02" do |web02|
        web02.vm.box = "jacobw/fedora35-arm64"
        web02.vm.hostname = "web02"
        web02.vm.network "private_network", ip: "192.168.10.4"
      end
  end