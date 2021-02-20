# -*- mode: ruby -*-
# vi: set ft=ruby :

ENV["VAGRANT_DEFAULT_PROVIDER"] ||= "docker"
Vagrant.configure(2) do |config|

    config.vm.provider(:docker) do |d|
            d.build_dir = "."
            d.has_ssh = true
            d.volumes = ["-v /var/run/docker.sock:/var/run/docker.sock"]
    end
end
  