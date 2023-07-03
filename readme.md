# :cloud: This repository features sample files to create a shared services cluster in EKS Anywhere
### :heavy_exclamation_mark: Apply the changes before applying the files via Kustomize or GitOps
The set of templates will deploy:
* External snapshotter
* PowerStore CSI drivers
* PowerStore Storage class and volumesnaphotclass
* MetalLB and related configuration
* NGINX Ingress controller
* PowerProtect Data Manager Service Account and RBAC
* Cluster Autoscaler
```
grep -rl EKSA_CLUSTER_NAME . | xargs sed -i "s/EKSA_CLUSTER_NAME/$CLUSTER_NAME/g"
```
