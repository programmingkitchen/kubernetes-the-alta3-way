# Kubernetes The Alta3 Way

This playbook walks you through setting up Kubernetes the Alta3 way. This guide is a fully automated command to bring up a Kubernetes cluster using Ansible.

Kubernetes The Alta3 Way is optimized for learning, which means taking the long route to ensure you understand each task required to bootstrap a Kubernetes cluster.

Kubernetes The Alta3 Way is used extensively within the student lab environments for Alat3's [Kubernetes Bootcamp](https://alta3.com/overview-k8s).  In this course each student has access to their own high availability Kubernetes environment capable of demonstrating all of the “K8s” features and components used in CKAD and CKA certifications (Certified Kubernetes Application Developer, Certified Kubernetes Administrator).

## Copyright

<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png" /></a><br />This work is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/">Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License</a>.

## Target Audience

The target audience for this tutorial is someone planning to support a production Kubernetes cluster and wants to understand how everything fits together.

## Cluster Details

Kubernetes The Alta3 Way guides you through bootstrapping a highly available Kubernetes cluster with:
* A highly available control plane backed by etcd
* End-to-end TLS encryption between components
* RBAC authenticated services and users
* Isolated and default-deny networking

Components and versions:

* [kubernetes](https://github.com/kubernetes/kubernetes) [1.23.3](https://kubernetes.io/releases/#release-v1-23)
* [containerd](https://github.com/containerd/containerd) [1.5.9](https://github.com/containerd/containerd/releases/tag/v1.5.9)
* [coredns](https://github.com/coredns/coredns) [v1.8.7](https://github.com/coredns/coredns/releases/tag/v1.8.7)
* [cni](https://github.com/containernetworking/cni) [v1.0.1](https://github.com/containernetworking/cni/releases/tag/v1.0.1)
* [calico](https://www.projectcalico.org/) [v3.21.4](https://github.com/projectcalico/calico/releases/tag/v3.21.4)
* [etcd](https://github.com/coreos/etcd) [v3.5.1](https://github.com/etcd-io/etcd/releases/tag/v3.5.1)
* [cfssl](https://github.com/cloudflare/cfssl) [v1.6.1](https://github.com/cloudflare/cfssl/releases/tag/v1.6.1)

