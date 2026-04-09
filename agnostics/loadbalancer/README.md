# MetalLB for K8TRE

This directory contains the Kubernetes manifests for deploying a loadbalancer for K8TRE. 

Learn more at [https://metallb.universe.tf/](https://metallb.universe.tf/)

## Structure

- `k3s/` - K3S-specific configurations including IP address pool definitions
- `aws/` - AWS-specific manifests.

## Vendor Differences

MetalLB is primarily used in K3S deployments for load balancing. 
Azure deployments typically use native Azure Load Balancer services instead and for K8TRE this is implemented through terraform (https://github.com/k8tre/k8tre-azure).
AWS EKS Loadbalancer manifests are in the `aws/` folder.
