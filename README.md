# MiniOLCNE - Oracle Linux Cloud Native Environment (mini version)
Thist is the MiniOLCNE Vagrant Box repository

The first step is to clone this repository:

    git clone https://github.com/osmarleao/miniolcne

Use this [VagrantFile](https://github.com/osmarleao/miniolcne/blob/master/Vagrantfile) to deploy your miniOLCNE:

    vagrant up

After the VM is up and running, you need to wait about 10 minutes to Kubernetes to boot.

Use the [kubeconfig](https://github.com/osmarleao/miniolcne/blob/master/kubeconfig) file to access your Kubernetes cluster:

    kubectl --kubeconfig kubeconfig get pods -A

To install a kubectl command, follow these instructions: https://kubernetes.io/docs/tasks/tools/install-kubectl/

