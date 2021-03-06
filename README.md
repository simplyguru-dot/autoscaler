# Kubernetes Autoscaler

[![Build Status](https://travis-ci.org/kubernetes/autoscaler.svg?branch=master)](https://travis-ci.org/kubernetes/autoscaler) [![GoDoc Widget]][GoDoc]

This repository contains autoscaling-related components for Kubernetes.

## What's inside

[Cluster Autoscaler](https://github.com/kubernetes/autoscaler/tree/master/cluster-autoscaler) - a component that automagically adjusts the size of a Kubernetes
Cluster so that all pods have a place to run and there are no unneeded nodes. Works with GCP, AWS and Azure. Current state - late beta, moving towards GA.

[Vertical Pod Autoscaler](https://github.com/kubernetes/autoscaler/tree/master/vertical-pod-autoscaler) - a set of components to automagically adjust the
amount of CPU and memory requested by pods running in the Kubernetes Cluster. Current state - under development.

[Addon Resizer](https://github.com/kubernetes/autoscaler/tree/master/addon-resizer) - a simplified version of vertical pod autoscaler that modifies
resource requests of a deployment based on the number of nodes in the Kubernetes Cluster. Current state - beta.

## Contact Info

Interested in autoscaling? Want to talk? Have questions, concenrns or great ideas?

Please join us on #sig-autoscaling at https://kubernetes.slack.com/.
Moreover, every Thursday we host a 30min sig-autoscaling meeting on
https://hangouts.google.com/hangouts/_/google.com/sig-autoscaling at
17:30 CEST/CET,  8:30 am PST/PDT.

## Getting the Code

The code must be checked out as a subdirectory of `k8s.io`, and not `github.com`.

```shell
mkdir -p $GOPATH/src/k8s.io
cd $GOPATH/src/k8s.io
# Replace "$YOUR_GITHUB_USERNAME" below with your github username
git clone https://github.com/$YOUR_GITHUB_USERNAME/autoscaler.git
cd autoscaler
```

[GoDoc]: https://godoc.org/k8s.io/autoscaler
[GoDoc Widget]: https://godoc.org/k8s.io/autoscaler?status.svg
