# Vagrant Kubernetes Cluster
Multi-nodes kubernetes cluster using vagrant and kubeadm for local experiments

## Prerequisites
- at least a 4 cores CPU and 8 GB RAM and 40 GB free disk space
- vagrant 2.2.5+
- virtualbox 6.0.10+
- make

## Install
`make install` Provision the VMs and setup the cluster (see vagrant/Vagrantfile)

## Clean
`make clean` Delete all nodes

## Use the cluster
1. `make ssh` Connect to the master node
2. Run `git clone https://github.com/Thomas-Webber/vagrant-kubernetes-cluster.git && cd vagrant-kubernetes-cluster`
to get the sources in the master node
3. `make install-helm` Install helm
4. `make install-prometheus` Install prometheus and grafana for monitoring

## Notes
Tested on OSX and Ubuntu Bionic
