# kubelet for 源码阅读

Implements [KEP 14 - Moving ComponentConfig API types to staging repos](https://git.k8s.io/enhancements/keps/sig-cluster-lifecycle/0014-20180707-componentconfig-api-types-to-staging.md#kubelet-changes)

This repo provides external, versioned ComponentConfig API types for configuring the kubelet.
These external types can easily be vendored and used by any third-party tool writing Kubernetes
ComponentConfig objects.

## Compatibility

HEAD of this repo will match HEAD of k8s.io/apiserver, k8s.io/apimachinery, and k8s.io/client-go.

## Where does it come from?

This repo is synced from https://github.com/kubernetes/kubernetes/tree/master/staging/src/k8s.io/kubelet.
Code changes are made in that location, merged into `k8s.io/kubernetes` and later synced here by a bot.
