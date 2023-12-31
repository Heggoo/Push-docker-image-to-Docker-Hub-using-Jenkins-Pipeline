Vagrant.configure("2") do |config|
  
	config.vm.define "jnk" do |jnk|
  
		jnk.vm.box = "ubuntu/focal64"
		jnk.vm.hostname = "jnk"
		jnk.vm.network "private_network", ip: "192.168.56.15"
		jnk.ssh.insert_key = false
		jnk.vm.provider "virtualbox" do |vb|
			vb.memory = "4000"
			vb.cpus = 2
		end
   
	jnk.vm.provision "shell", path:"jenkins.sh"
	end
end