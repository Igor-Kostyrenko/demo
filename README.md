| NAME | PROMPT | DESCRIPTION | EXAMPLE |
|------|--------|-------------|---------|
| Pod | Create a YAML manifest for a Pod. | Define a single instance of a containerized application. | [YAML Example](yaml/app-pod.yaml) |
| Deployment | Create a YAML manifest for a Deployment. | Define a declarative way to manage a set of replicated Pods. | [YAML Example](/workspaces/demo/yaml/app-deployment.yaml) |
| Service | Create a YAML manifest for a Service. | Expose an application running on a set of Pods as a network service. | [YAML Example](yaml/app-configmap.yaml)) |
| Ingress | Create a YAML manifest for an Ingress. | Configure external access to services in a cluster. | [YAML Example](https://kubernetes.io/docs/concepts/services-networking/ingress/#simple-fanout) |
| ConfigMap | Create a YAML manifest for a ConfigMap. | Store non-confidential data as key-value pairs. | [YAML Example](yaml/app-configmap.yaml)) |
| Secret | Create a YAML manifest for a Secret. | Store confidential data, such as passwords or API keys. | [YAML Example](https://kubernetes.io/docs/concepts/configuration/secret/#using-secrets) |
| PersistentVolume | Create a YAML manifest for a PersistentVolume. | Allocate durable storage in a cluster. | [YAML Example](https://kubernetes.io/docs/concepts/storage/persistent-volumes/#persistentvolume-example) |
| PersistentVolumeClaim | Create a YAML manifest for a PersistentVolumeClaim. | Request storage resources from a PersistentVolume. | [YAML Example](https://kubernetes.io/docs/concepts/storage/persistent-volumes/#persistentvolumeclaim-example) |
| Job | Create a YAML manifest for a Job. | Run a task or a batch job to completion. | [YAML Example](https://kubernetes.io/docs/concepts/workloads/controllers/job/#creating-a-job) |
| CronJob | Create a YAML manifest for a CronJob. | Schedule a job to run periodically at a specified time or interval. | [YAML Example](https://kubernetes.io/docs/concepts/workloads/controllers/cron-jobs/#creating-a-cron-job) |

