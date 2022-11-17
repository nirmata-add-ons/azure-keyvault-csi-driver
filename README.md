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
2. Create a Nirmata catalog application with a Git upstream and select the azure-keyvault-csi-driver repository. You can optionally select the kustomization.
3. 
