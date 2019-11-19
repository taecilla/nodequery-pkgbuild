Vagrant.configure("2") do |config|
  config.vm.box = "taecilla/arch-linux"
	config.vm.hostname = "NodeQuery"

	config.vm.provision "shell", inline: "sudo pacman -Syu base-devel --noconfirm"
	config.vm.provision "shell", inline: "sudo pacman -Syu --noconfirm", run: "always"

	config.vm.provider "virtualbox" do |v|
		v.name = "NodeQuery"
	end

	config.ssh.insert_key = false
end
