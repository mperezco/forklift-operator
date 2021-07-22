# Konveyor Forklift Operator

Konveyor Forklift Operator installs a suite of migration tools that facilitate the migration of VM workloads to KubeVirt

## Prerequisites

* __KubeVirt 0.42__

## Konveyor Forklift Operator Installation

Konveyor Forklift Operator is not yet available in OperatorHub.io

### Installing 

Installing requires having Kubernetes with OLM installed as well as having ingress router deployed

1. Create namespace `kubectl namespace create my-forklift-operator`
1. Create operator `kubectl create -f forklift-operator-catalog-kube.yaml`
1. Create operator group `kubectl create -f forklift-operator-group-kube.yaml`
1. Instantiate operator `kubectl create -f forklift-operator-crd-kube.yaml`

## Customize Settings

Custom settings can be applied by editing the `ForkliftController` CR.

`kubectl edit forkliftcontroller -n my-forklift-operator`

## Forklift Documentation

See the [Konveyor Forklift Documentation](https://forklift-docs.konveyor.io/) for detailed installation instructions as well as how to use Konveyor Forklift.
