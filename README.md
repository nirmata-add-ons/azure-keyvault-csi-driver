# azure-keyvault-csi-driver

## The Azure Key Vault Provider for Secrets Store CSI Driver in an AKS cluster

The Azure Key Vault Provider for Secrets Store CSI Driver allows for the integration of an Azure key vault as a secret store with an Azure Kubernetes Service (AKS) cluster via a CSI volume.

## Features

Mounts secrets, keys, and certificates to a pod by using a CSI volume
Supports CSI inline volumes
Supports mounting multiple secrets store objects as a single volume
Supports pod portability with the SecretProviderClass CRD
Supports Windows containers
Syncs with Kubernetes secrets
Supports auto rotation of mounted contents and synced Kubernetes secrets

## How do I get set up?

1. Clone this repository or add its contents to your own private Git repository.
2. Create a Nirmata catalog application with a Git upstream and select the **azure-keyvault-csi-driver** repository and choose **csi-driver-for-linux-v1.3.0** branch for linux nodes and choose **csi-driver-for-windows-v1.3.0** branch for windows nodes. You can optionally select the kustomization. In Advanced section add **kube-system" namespace. Then Choose the **Security** as a Add-on Category.
3. Update a Cluster Type, or create a new one, and select the **azure-keyvault** add-on application in the "Add-Ons" section. Ensure that the namespace you use is "kube-system" and environment is "kube-system-< cluster-name >"
4. Create clusters using the cluster type.
5. If addon is to be added to a running cluster, choose a environemnt with namespace **"kube-system-< cluster-name >"** and choose this environment while deploying the application
6. Verify that the application is running.

## Who do I talk to?
For issues, contact support@nirmata.com

