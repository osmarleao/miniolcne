# MiniOLCNE - Oracle Linux Cloud Native Environment (mini version)
Thist is the MiniOLCNE Vagrant Box repository

The first step is to clone this repository:

      git clone https://github.com/osmarleao/miniolcne

There are some requirements before you use VagrantFile to deploy your miniOLCNE box:

* Configure one Host-Only Interface on your VirtualBOX with an IP address inside 172.31.188.0/24 network (excluding 172.31.188.1);

* Use this interface name on `VagrantFile` like example below:

      config.vm.network "private_network", ip: "172.31.188.1",
        name: "vboxnet"
      config.vm.hostname = "miniolcne.br.olsclab.net"

* 
