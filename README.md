# Kube Kind Cluster

Configs to setup kube cluster using kind.

## Prerequisites

- docker
- [kind](https://kind.sigs.k8s.io)

## Overview

- [master-only.yaml](master-only.yaml) will create a k8s cluster with only single master node.
- [master-only-with-port-mapping.yaml](master-only-master-only-with-port-mapping.yaml) will create a k8s cluster with only single master node and port mappings on the host for access.
- [multi-node.yaml](multi-node.yaml) will create a k8s cluster with 1 master and 2 worker nodes.
  
## Usage

- Run the following command to create a cluster
    ```shell
    kind create cluster --name <cluster-name> --config <config.yaml>
    ```
- The config.yaml can be one of the configs mentioned above.

## More Information

- For more information on various configurations visit https://kind.sigs.k8s.io