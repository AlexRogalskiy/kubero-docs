# Prerequisites
In order to install Kubero, you need to have a Kubernetes cluster and the `kubectl` command line tool installed.

## Kubernetes cluster
You can use any Kubernetes cluster. If you don't have access to a Kubernetes cluster, you have a few options. One option is to use [Kind](https://kind.sigs.k8s.io/docs/user/quick-start/) to start a cluster on your desktop. Alternatively, you can use the Kubero CLI to create a cluster on one of the many cloud providers that offer Kubernetes as a service.

### Starting a local Kind cluster

```bash
wget https://raw.githubusercontent.com/kubero-dev/kubero/main/kind.yaml
kind create cluster --config kind.yaml
```
