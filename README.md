# Dispatch Addon Repository

This is a [kubernetes addon](https://github.com/mesosphere/kubeaddons) repository which contains the [Dispatch](https://github.com/mesosphere/dispatch) addon.

## Releasing New Dispatch Versions

This repository is automatically updated by the [Dispatchfile](https://github.com/mesosphere/dispatch/blob/dev/Dispatchfile) of the Dispatch repository
when a new Dispatch release is tagged.

## Images Required by Air-gapped Environments

Most images can be fetched through helm test. However, the following images needs to be added manually with proper tags at the moment:

- System images from https://github.com/mesosphere/dispatch/blob/dev/charts/dispatch/charts/tekton/values.yaml:
  - `gcr.io/tekton-releases/github.com/tektoncd/pipeline/cmd/kubeconfigwriter`
  - `gcr.io/tekton-releases/github.com/tektoncd/pipeline/cmd/pullrequest-init`
  - `gcr.io/tekton-releases/github.com/tektoncd/pipeline/vendor/github.com/googlecloudplatform/cloud-builders/gcs-fetcher/cmd/gcs-fetcher`
  - `docker.io/tianon/true`
  - `docker.io/nginx`
- CLI images
  - `docker.io/mesosphere/dispatch-argocd`
  - `docker.io/mesosphere/tkn`
  - `docker.io/mesosphere/dispatch-helm`
- Utility images
  - `docker.io/mesosphere/update-gitops-repo`
  - `docker.io/mesosphere/dispatch-dind`
