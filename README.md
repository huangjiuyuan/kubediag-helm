# KubeDiag Helm

This Helm chart installs KubeDiag in a Kubernetes cluster.

## Prerequisites

Please make sure the enviroment for installing KubeDiag fulfills the following requirements:

* [Kubernetes](https://github.com/kubernetes/kubernetes) 1.16+
* [Helm](https://github.com/helm/helm) 3.0+
* [Cert Manager](https://github.com/jetstack/cert-manager) 1.0+

## Installation

Run the following command to install KubeDiag via Helm:

```bash
helm install kubediag --create-namespace --namespace kubediag ./
```

Check the status of KubeDiag by running the command:

```bash
kubectl get all --namespace kubediag
```

## Uninstallation

Run the following command to install KubeDiag via Helm:

```bash
helm uninstall --namespace kubediag kubediag
```