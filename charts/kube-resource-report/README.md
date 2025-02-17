# kube-resource-report

![Version: 0.0.7](https://img.shields.io/badge/Version-0.0.7-informational?style=flat-square) ![Type: application](https://img.shields.io/badge/Type-application-informational?style=flat-square) ![AppVersion: 21.2.1](https://img.shields.io/badge/AppVersion-21.2.1-informational?style=flat-square)

Helm chart to deploy [kube-resource-report](https://codeberg.org/hjacobs/kube-resource-report).

**Homepage:** <https://github.com/slamdev/helm-charts/tree/master/charts/kube-resource-report>

## Maintainers

| Name | Email | Url |
| ---- | ------ | --- |
| slamdev | valentin.fedoskin@gmail.com |  |

## Values

| Key | Type | Default | Description |
|-----|------|---------|-------------|
| affinity | object | `{}` | affinity for scheduler pod assignment |
| app.resources | object | `{}` | custom resource configuration |
| args | list | `[]` | extra args to pass to container |
| env | string | `nil` | environment variables for the deployment |
| fullnameOverride | string | `""` | full name of the chart. |
| image.pullPolicy | string | `"IfNotPresent"` | image pull policy |
| image.repository | string | `"hjacobs/kube-resource-report"` | image repository |
| image.tag | string | `""` | image tag (chart's appVersion value will be used if not set) |
| imagePullSecrets | list | `[]` | image pull secret for private images |
| ingress.annotations | object | `{}` | ingress annotations |
| ingress.enabled | bool | `false` | enables Ingress for kube-resource-report |
| ingress.hosts | list | `[]` | ingress accepted hostnames |
| ingress.tls | list | `[]` | ingress TLS configuration |
| nameOverride | string | `""` | override name of the chart |
| nginx.resources | object | `{}` | custom resource configuration |
| nodeSelector | object | `{}` | node for scheduler pod assignment |
| podSecurityContext | object | `{}` | specifies security settings for a pod |
| pricingData | string | `"dc-1,master,30.000\ndc-1,worker,500.000"` | CSV with columns region,instance-type,monthly-price-usd |
| service.port | int | `80` | service port |
| service.type | string | `"ClusterIP"` | service type |
| serviceAccount.annotations | object | `{}` | annotations to add to the service account |
| serviceAccount.create | bool | `false` | specifies whether a service account should be created |
| serviceAccount.name | string | `nil` | the name of the service account to use; if not set and create is true, a name is generated using the fullname template |
| tolerations | list | `[]` | tolerations for scheduler pod assignment |
| volumeMounts | string | `nil` | volume mounts |
| volumes | string | `nil` | volumes |
