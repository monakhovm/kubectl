# Kubernetes Prompt Portfolio

This repository contains a portfolio of English prompts for generating and analyzing Kubernetes manifests. Each prompt is designed according to best practices in prompt engineering and can be used with tools like [kubectl-ai](https://github.com/GoogleCloudPlatform/kubectl-ai).

| NAME                 | PROMPT                                                                 | DESCRIPTION                                                   | EXAMPLE                |
|----------------------|------------------------------------------------------------------------|---------------------------------------------------------------|------------------------|
| app.yaml             | Generate a basic Kubernetes Deployment manifest for a Go web app named "demo-app" with image "denvash/go-demo-app:1.0". | Basic deployment for Go demo app.                             | [yaml/app.yaml](yaml/app.yaml) |
| app-livenessProbe.yaml | Generate a Kubernetes Deployment manifest for "demo-app" with a liveness probe that checks "/healthz" on port 8080. | Deployment with liveness probe for health checking.           | [yaml/app-livenessProbe.yaml](yaml/app-livenessProbe.yaml) |
| app-readinessProbe.yaml | Generate a Kubernetes Deployment manifest for "demo-app" with a readiness probe that checks "/ready" on port 8080. | Deployment with readiness probe.                              | [yaml/app-readinessProbe.yaml](yaml/app-readinessProbe.yaml) |
| app-volumeMounts.yaml | Generate a Deployment manifest for "demo-app" with a volume mount for persistent data at "/data". | Deployment with volume mount.                                 | [yaml/app-volumeMounts.yaml](yaml/app-volumeMounts.yaml) |
| app-cronjob.yaml     | Generate a Kubernetes CronJob manifest to run "demo-app" every day at midnight. | CronJob for scheduled execution.                              | [yaml/app-cronjob.yaml](yaml/app-cronjob.yaml) |
| app-job.yaml         | Generate a Kubernetes Job manifest to run a one-time "demo-app" container. | Job for one-time execution.                                   | [yaml/app-job.yaml](yaml/app-job.yaml) |
| app-multicontainer.yaml | Generate a Deployment manifest for "demo-app" with two containers: "main" and "sidecar". | Deployment with multiple containers.                          | [yaml/app-multicontainer.yaml](yaml/app-multicontainer.yaml) |
| app-resources.yaml   | Generate a Deployment manifest for "demo-app" with resource requests and limits (cpu: 100m/200m, memory: 128Mi/256Mi). | Deployment with resource limits.                              | [yaml/app-resources.yaml](yaml/app-resources.yaml) |
| app-secret-env.yaml  | Generate a Deployment manifest for "demo-app" that uses a secret as environment variable "MY_SECRET". | Deployment with secret environment variable.                 | [yaml/app-secret-env.yaml](yaml/app-secret-env.yaml) |

## How to use

- Copy any prompt from the table and use it with [kubectl-ai](https://github.com/GoogleCloudPlatform/kubectl-ai) or another LLM-powered tool to generate or analyze Kubernetes manifests.
- Each EXAMPLE links to a sample manifest in the `yaml/` directory.

## Prompt Engineering Best Practices

- Use clear, concise, and action-oriented prompts.
- Specify output format (YAML, JSON, etc.).
- Include resource names, images, ports, and additional options as needed.
- Test prompts and iterate for best results.
