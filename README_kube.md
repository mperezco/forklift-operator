# Konveyor Forklift Operator

Konveyor Forklift Operator installs a suite of migration tools that facilitate the migration of VM workloads to KubeVirt

## Prerequisites

* __KubeVirt 0.42__

## Konveyor Forklift Operator Installation

Konveyor Forklift Operator is not yet available in OperatorHub.io

### Installing _latest_

Installing latest is almost an identical procedure to released versions but requires creating a new catalog source.

1. Create namespace `kubectl namespace create my-forklift-operator`
1. Create operator `kubectl create -f forklift-operator-catalog-kube.yaml`
1. ???

**Note:** Installing _Latest_ will also include OLM channels for released versions.

## Customize Settings

Custom settings can be applied by editing the `ForkliftController` CR.

`kubectl edit forkliftcontroller -n my-forklift-operator`

## Forklift Documentation

See the [Konveyor Forklift Documentation](https://forklift-docs.konveyor.io/) for detailed installation instructions as well as how to use Konveyor Forklift.
