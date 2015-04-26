# Example 4
#
# Single box with Apache and sample static site installed via Puppet.
#

Vagrant.configure("2") do |config|
  config.vm.box = "hashicorp/precise32"
  config.vm.host_name = "myprecisebox.example.com"
  config.vm.network "private_network",  ip: "192.168.0.42"

  config.vm.provision "puppet" do |puppet|
    puppet.manifests_path = "puppet/manifests"
    puppet.manifest_file = "site.pp"
    puppet.module_path = "puppet/modules"
  end
end
