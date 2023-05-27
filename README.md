| NAME                  | PROMPT                                           | DESCRIPTION                                                         | EXAMPLE                                                            |
|-----------------------|--------------------------------------------------|---------------------------------------------------------------------|--------------------------------------------------------------------|
| app.yaml              | Manifest for creating a Kubernetes Pod     | This manifest defines a Deployment resource for an application       | [app.yaml example](yaml/app.yaml)                    |
| app-livenessProbe.yaml | Manifest for configuring liveness probe           | This manifest demonstrates how to configure a liveness probe        | [app-livenessProbe.yaml example](yaml/app-livenessProbe.yaml) |
| app-readinessProbe.yaml| Manifest for configuring readiness probe          | This manifest demonstrates how to configure a readiness probe       | [app-readinessProbe.yaml example](yaml/app-readinessProbe.yaml) |
| app-volumeMounts.yaml  | Manifest for defining volume mounts               | This manifest shows how to define volume mounts for a container     | [app-volumeMounts.yaml example](yaml/app-volumeMounts.yaml) |
| app-cronjob.yaml      | Manifest for creating a Kubernetes CronJob        | This manifest creates a CronJob resource for running scheduled tasks| [app-cronjob.yaml example](yaml/app-cronjob.yaml)    |
| app-job.yaml          | Manifest for creating a Kubernetes Job            | This manifest defines a Job resource for running a one-time task    | [app-job.yaml example](yaml/app-job.yaml)            |
| app-multicontainer.yaml| Manifest for creating a Pod with multiple containers| This manifest shows how to define a Pod with multiple containers    | [app-multicontainer.yaml example](yaml/app-multicontainer.yaml) |
| app-resources.yaml    | Manifest for configuring resource limits          | This manifest demonstrates how to set resource limits for a container | [app-resources.yaml example](yaml/app-resources.yaml) |
| app-secret-env.yaml   | Manifest for using a Secret as environment variables| This manifest shows how to use a Secret to populate environment variables | [app-secret-env.yaml example](yaml/app-secret-env.yaml) |

