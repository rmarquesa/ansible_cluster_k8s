# Project to learn..
### Build a k8s cluster using playbook ansible
Project to use in CentOS/Red Hat/Oracle Linux distribuition


**1 - Creating non-root user with sudo privileges**
```sh
ansible-playbook -i k8s_inventory.ini ~/ansible_cluster_k8s/create_non_root_sudo_user.yaml
```

**2 - Installing k8s depedencies**
```sh
ansible-playbook -i k8s_inventory.ini ~/ansible_cluster_k8s/k8s_dependencies.yaml
```

**3 - Installing k8s depedencies**
```sh
ansible-playbook -i k8s_inventory.ini ~/ansible_cluster_k8s/k8s_dependencies.yaml
```

**4 - Configure Node Master**
```sh
ansible-playbook -i k8s_inventory.ini ~/ansible_cluster_k8s/k8s_dependencies.yaml
```

**5 - Configure Nodes Workers**
```sh
ansible-playbook -i k8s_inventory.ini ~/ansible_cluster_k8s/k8s_workers.yaml
```

### References
 - https://kubernetes.io/pt-br/docs/setup/production-environment/tools/kubeadm/install-kubeadm/
 - https://www.digitalocean.com/community/tutorials/como-criar-um-cluster-kubernetes-1-10-usando-kubeadm-no-centos-7-pt
 - https://github.com/flannel-io/flannel#flannel