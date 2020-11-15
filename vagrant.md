## VagrantFile
```java 

Vagrant.configure("2") do |config|
  # Every Vagrant virtual environment requires a box to build off of.
  config.vm.box = "centos/7"
  
  # Create a forwarded port mapping which allows access to a specific port
  # within the machine from a port on the host machine. In the example below,
  # accessing "localhost:8080" will access port 80 on the guest machine.
  config.vm.network "forwarded_port", guest: 80, host: 8080
  
  # If true, then any SSH connections made will enable agent forwarding.
  # Default value: false
  # config.ssh.forward_agent = true
  
  # Mentioning the SSH Username/Password:
	config.ssh.username = "vagrant"
	config.ssh.password = "vagrant"

  #config.vagrant.plugins = ["vagrant-plugin", "vagrant-other-plugin"]
end
```
