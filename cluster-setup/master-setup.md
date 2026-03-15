# Master Node Setup

The Kubernetes control plane was initialized using kubeadm.

Initialize cluster:

sudo kubeadm init --pod-network-cidr=10.244.0.0/16

Configure kubectl:

mkdir -p $HOME/.kube
sudo cp /etc/kubernetes/admin.conf $HOME/.kube/config
sudo chown $(id -u):$(id -g) $HOME/.kube/config

Install Flannel network plugin:

kubectl apply -f https://raw.githubusercontent.com/flannel-io/flannel/master/Documentation/kube-flannel.yml

Verify cluster:

kubectl get nodes

