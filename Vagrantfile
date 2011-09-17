Vagrant::Config.run do |config|

  config.vm.define :chef_quick_start do |chef_quick_start|

    chef_quick_start.vm.customize do |vm|
      vm.name = "Chef Quick Start"
    end

    chef_quick_start.vm.box = "base"

    chef_quick_start.vm.network "33.33.33.31"

    chef_quick_start.vm.provision :shell do |shell|
      shell.path = "scripts/set_fqdn.sh"
      shell.args = "quick-start.chef.tw"
    end
  end
end
