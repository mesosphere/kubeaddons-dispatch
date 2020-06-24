# Dispatch Addon Repository

This is a [kubernetes addon](https://github.com/mesosphere/kubeaddons) repository which contains the [Dispatch](https://github.com/mesosphere/dispatch) addon.

## Releasing New Dispatch Versions

This repository is automatically updated by the [Dispatchfile](https://github.com/mesosphere/dispatch/blob/dev/Dispatchfile) of the Dispatch repository
when a new Dispatch release is tagged.

## Images Required by Air-gapped Environments

Most images can be fetched through helm test. However, the following images needs to be added manually at the moment:

- Parser images for Dispatch 1.0
  - `mesosphere/dispatch-starlark:v0.1`
  - `mesosphere/dispatch-cue:v0.1`
  - `mesosphere/dispatch-yaml:v0.1`
  - `mesosphere/dispatch-json:v0.1`
- Parser images for Dispatch 1.1
  - `mesosphere/dispatch-starlark:v0.5`
  - `mesosphere/dispatch-cue:v0.2`
  - `mesosphere/dispatch-yaml:v0.2`
  - `mesosphere/dispatch-json:v0.2`
- Parser images for Dispatch 1.2
  - `mesosphere/dispatch-starlark:v0.6`
  - `mesosphere/dispatch-cue:v0.4`
  - `mesosphere/dispatch-yaml:v0.3`
  - `mesosphere/dispatch-json:v0.3`
- Utility images
  - `mesosphere/update-gitops-repo:1.2.0`
