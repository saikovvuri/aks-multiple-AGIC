# Azure Kubernetes Service (AKS) cluster configured with multiple Application Gateway Ingress Controllers (AGIC) (1 public and other private front end IP) depoyed via Helm Chart
AKS with configured with two Application Gateway Ingress Controllers (AGIC) - 1 public and other private front end IP, deployed through helm chart, each one pointing to a different application gateway

## Provision azure resources

```bash
export subscriptionId=$(az acccount show --query id --output tsv)
./aks-2agic-helm.azcli

## Architecture

![aks-multiple-agic.PNG](/aks-multiple-agic.PNG)
