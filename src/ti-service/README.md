# ti-service

![Version: 0.2.9](https://img.shields.io/badge/Version-0.2.9-informational?style=flat-square) ![Type: application](https://img.shields.io/badge/Type-application-informational?style=flat-square) ![AppVersion: 0.0.1](https://img.shields.io/badge/AppVersion-0.0.1-informational?style=flat-square)

A Helm chart for Kubernetes

## Requirements

| Repository | Name | Version |
|------------|------|---------|
| https://harness.github.io/helm-common | harness-common | 1.x.x |

## Values

| Key | Type | Default | Description |
|-----|------|---------|-------------|
| affinity | object | `{}` |  |
| autoscaling.enabled | bool | `true` |  |
| autoscaling.maxReplicas | int | `100` |  |
| autoscaling.minReplicas | int | `1` |  |
| autoscaling.targetCPUUtilizationPercentage | int | `80` |  |
| fullnameOverride | string | `""` |  |
| global.loadbalancerURL | string | `""` |  |
| image.digest | string | `""` |  |
| image.pullPolicy | string | `"IfNotPresent"` |  |
| image.registry | string | `"docker.io"` |  |
| image.repository | string | `"harness/ti-service-signed"` |  |
| image.tag | string | `"release-77"` |  |
| imagePullSecrets | object | `{}` |  |
| jobresources.limits.cpu | int | `1` |  |
| jobresources.limits.memory | string | `"3072Mi"` |  |
| jobresources.requests.cpu | int | `1` |  |
| jobresources.requests.memory | string | `"3072Mi"` |  |
| jobs.migrate.image.digest | string | `""` |  |
| jobs.migrate.image.pullPolicy | string | `"IfNotPresent"` |  |
| jobs.migrate.image.registry | string | `"docker.io"` |  |
| jobs.migrate.image.repository | string | `"harness/ti-service-signed"` |  |
| jobs.migrate.image.tag | string | `"release-77"` |  |
| maxSurge | int | `1` |  |
| maxUnavailable | int | `0` |  |
| mongoSecrets.password.key | string | `"mongodbPassword"` |  |
| mongoSecrets.password.name | string | `"harness-secrets"` |  |
| mongoSecrets.userName.key | string | `"mongodbUsername"` |  |
| mongoSecrets.userName.name | string | `"harness-secrets"` |  |
| nameOverride | string | `""` |  |
| nodeSelector | object | `{}` |  |
| podAnnotations | object | `{}` |  |
| podSecurityContext | object | `{}` |  |
| replicaCount | int | `1` |  |
| resources.limits.cpu | int | `1` |  |
| resources.limits.memory | string | `"3072Mi"` |  |
| resources.requests.cpu | int | `1` |  |
| resources.requests.memory | string | `"3072Mi"` |  |
| securityContext.runAsNonRoot | bool | `true` |  |
| securityContext.runAsUser | int | `65534` |  |
| service.port | int | `8078` |  |
| service.type | string | `"ClusterIP"` |  |
| serviceAccount.annotations | object | `{}` |  |
| serviceAccount.create | bool | `false` |  |
| serviceAccount.name | string | `"harness-default"` |  |
| tiServiceTimescaleSecret.password.key | string | `"timescaledbPostgresPassword"` |  |
| tiServiceTimescaleSecret.password.name | string | `"harness-secrets"` |  |
| tolerations | list | `[]` |  |
| useSSL | bool | `false` |  |
| waitForInitContainer.image.digest | string | `""` |  |
| waitForInitContainer.image.pullPolicy | string | `"IfNotPresent"` |  |
| waitForInitContainer.image.registry | string | `"docker.io"` |  |
| waitForInitContainer.image.repository | string | `"harness/helm-init-container"` |  |
| waitForInitContainer.image.tag | string | `"latest"` |  |

