#Controlplan node

kubectl drain controlplane --ignore-daemonsets

apt-get update

apt-get upgrade kubeadm=1.27.0-00

kubeadm upgrade apply v1.27.0

apt-get install kubelet=1.27.0-00

systemctl daemon-reload

systemctl restart kubelet

#Worker node

kubectl drain node01 --ignore-daemonsets

apt-get install kubelet=1.27.0-00

systemctl daemon-reload

systemctl restart kubelet
