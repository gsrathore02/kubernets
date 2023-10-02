# Kubernets
```
Kubernetes is an open-source container orchestration system for automating software deployment, scaling, and management. Originally designed by Google, the project is now maintained by the Cloud Native Computing Foundation.
```
## Kubernetes Cluster
## Master Node
```
The master is the control plane of Kubernetes.
It consists of several components, such as an API server, a scheduler, and a controller manager.
The master is responsible for the global state of the cluster, cluster-level scheduling of pods, and handling of events. Usually, all the master components are set up on a single host.
When considering high-availability scenarios or very large clusters, you will want to have master redundancy.
```
## Worker Node
```
You can think of these as container clients.
These are individual hosts (physical or virtual) on which Docker would be installed to host different containers within your managed cluster
Each Node will run ETCD (key pair management and communication service, used by Kubernetes for exchanging messages and reporting Cluster status) as well as the Kubernetes proxy
```
