---
title: Frequently asked questions
menu_order: 95
search_type: Documentation
---

# Frequently asked questions

## Running Scope in a Kubernetes setting

A simple way to get Scope running in a Kubernetes setting is to

1. Clone the Scope repo:

   ```sh
   git clone https://github.com/weaveworks/scope
   cd scope
   ```

1. Spin up a cluster wherever it suits you.
   [Minikube](https://github.com/kubernetes/minikube) is a simple option.
1. Run

   ```sh
   kubectl apply -f example/k8s
   ```

   to deploy Scope to your cluster.
1. Port-forward to access `weave-scope-app`:

   ```sh
   kubectl port-forward svc/weave-scope-app -n weave 4040:80
   ```

1. Point your browser to <http://127.0.0.1:4040.>