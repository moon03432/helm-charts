# Helm chart repository

[Helm chart repository](https://github.com/kubernetes/helm/blob/master/docs/chart_repository.md) is an HTTP server that houses an `index.yaml` file and
optionally some packaged charts.  When you're ready to share your charts, the
preferred way to do so is by uploading them to a chart repository.

## Introduction

This chart bootstraps a [Helm chart repository](https://github.com/kubernetes/helm/blob/master/docs/chart_repository.md) deployment on a [Kubernetes](http://kubernetes.io) cluster using the [Helm](https://helm.sh) package manager.

## Installing the Chart

To install the chart with the release name `helm-repo`:

```console
$ helm install --name=helm-repo --namespace=kube-system --set ingress.host=helm.kubernetes.wanda.cn k8s/helm-repo
```

The command deploys helm-repo on the Kubernetes cluster with http://helm.kubernetes.wanda.cn/charts .

## Uninstalling the Chart

To uninstall/delete the `helm-repo` deployment:

```console
$ helm delete helm-repo
```

The command removes all the Kubernetes components associated with the chart and deletes the release.

## Configuration

The following tables lists the configurable parameters of the kubernetes-dashboard chart and their default values.

| Parameter      | Description    | Default |
| -------------- | -------------- | ------- |
| `ingress.host` | repository url | `nil`   |
Specify each parameter using the `--set key=value[,key=value]` argument to `helm install`. For example,

```console
$ helm install --name=helm-repo --namespace=kube-system --set ingress.host=helm.kubernetes.wanda.cn k8s/helm-repo
```

Alternatively, a YAML file that specifies the values for the above parameters can be provided while installing the chart. For example,

```console
$ helm install k8s/helm-repo --name my-release -f values.yaml
```

> **Tip**: You can use the default [values.yaml](values.yaml)

