#  Provision a GKE Private Cluster using Terraform

This repo is a companion repo to the [Provision a GKE Cluster tutorial](https://developer.hashicorp.com/terraform/tutorials/kubernetes/gke), containing Terraform configuration files to provision an GKE cluster on GCP. In addition this creates a complete private cluster.

Note: In order to access the Kubernetes API server and run kubectl commands , you cannot use regular way to access and need to be in the same VPC as the cluster. You should preferably using a VM that uses the custom vpc as the private cluster vpc in GCP.

This sample repo also creates a VPC and subnet for the GKE cluster. This is not
required but highly recommended to keep your GKE cluster isolated.
