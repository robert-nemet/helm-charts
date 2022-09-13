# Helm Charts

## Add Repository

```sh
helm repo add rnemet https://rnemet.dev/helm-charts
```

## Install

### Klock

[Locks for Kubernetes](https://github.com/robert-nemet/klock).

```sh
helm install klock rnemet/klock
```

It requires [`cert-manager`](https://cert-manager.io/) to be already present in the cluster.

