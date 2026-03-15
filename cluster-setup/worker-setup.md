# Worker Node Setup

Worker nodes join the cluster using kubeadm join.

Example command:


kubeadm join 192.168.142.131:6443 --token jm9kop.cp4q8hwsr6zt7tqc  --discovery-token-ca-cert-hash sha256:96f3c8456caf245dc3b8291a3fb4a75373de5f9153630831e2c5f57248602de5


Verification:

kubectl get nodes

