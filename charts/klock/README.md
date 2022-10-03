# PromLens

![Version: 1.0.1](https://img.shields.io/badge/Version-1.0.1-informational?style=flat-square) ![Type: application](https://img.shields.io/badge/Type-application-informational?style=flat-square) ![AppVersion: 2.0.0](https://img.shields.io/badge/AppVersion-2.0.0-informational?style=flat-square)

This chart installs [Klock](https://github.com/robert-nemet/klock).

Klock provides locks for Kubernetes.

## Helm Chart

### How To Install

Simply add this Chart repository to Helm:

```sh
➜ helm repo add rnemet https://rnemet.dev/helm-charts
```

## Values

| Key | Type | Default | Description |
|-----|------|---------|-------------|
| affinity | object | `{}` |  |
| config.operations[0] | string | `"DELETE"` |  |
| config.operations[1] | string | `"UPDATE"` |  |
| config.resources[0] | string | `"pods"` |  |
| config.resources[1] | string | `"deployments"` |  |
| config.resources[2] | string | `"secrets"` |  |
| config.resources[3] | string | `"configmaps"` |  |
| image.pullPolicy | string | `"IfNotPresent"` |  |
| image.repository | string | `"rnemet/klock"` |  |
| image.tag | string | `"2.0.0"` |  |
| imagePullSecrets | list | `[]` |  |
| label.klock-control-plane | string | `"klock-controller-manager"` |  |
| namespace.name | string | `"klock-system"` |  |
| nodeSelector | object | `{}` |  |
| replicaCount | int | `1` |  |
| resources.limits.cpu | string | `"100m"` |  |
| resources.limits.memory | string | `"64Mi"` |  |
| resources.requests.cpu | string | `"100m"` |  |
| resources.requests.memory | string | `"64Mi"` |  |
| tolerations | list | `[]` |  |

