# external-secrets-operator

![Version: 0.0.14](https://img.shields.io/badge/Version-0.0.14-informational?style=flat-square) ![Type: application](https://img.shields.io/badge/Type-application-informational?style=flat-square) ![AppVersion: 0.0.8](https://img.shields.io/badge/AppVersion-0.0.8-informational?style=flat-square)

Helm chart to deploy [external-secrets-operator](https://github.com/slamdev/external-secrets-operator).

External Secrets Operator watches changes in external key-value backends to sync them with Kubernetes Secrets and ConfigMaps.

Refer to operator repo for additional information.

**Homepage:** <https://github.com/slamdev/helm-charts/tree/master/charts/external-secrets-operator>

## Maintainers

| Name | Email | Url |
| ---- | ------ | --- |
| slamdev | valentin.fedoskin@gmail.com |  |

## Values

| Key | Type | Default | Description |
|-----|------|---------|-------------|
| affinity | object | `{}` | affinity for scheduler pod assignment |
| env | list | `[]` | additional environment variables for the deployment |
| fullnameOverride | string | `""` | full name of the chart. |
| image.pullPolicy | string | `"IfNotPresent"` | image pull policy |
| image.repository | string | `"slamdev/external-secrets-operator"` | image repository |
| image.tag | string | `""` | image tag (chart's appVersion value will be used if not set) |
| imagePullSecrets | list | `[]` | image pull secret for private images |
| nameOverride | string | `""` | override name of the chart |
| nodeSelector | object | `{}` | node for scheduler pod assignment |
| resources | object | `{}` | custom resource configuration |
| tolerations | list | `[]` | tolerations for scheduler pod assignment |
