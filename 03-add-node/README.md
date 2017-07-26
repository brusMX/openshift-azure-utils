# Add a node to your Openshift cluster

This util allows you to scale your cluster up. You need to provide the characteristics for your cluster.

## Proposed things to work on

1. Create script to set up VM with network configuration
1. Create script to call ansible script to add Node to cluster
1. Set up a dockerfile ready to use the libraries and tools for python on Azure
1. Publish docker image to deploy as a pod inside the Openshift that can manage the new pool of nodes.

## Run this

1. Create a `azureconfig.yaml` file from `azureconfig.yaml.backup` and fill it up wit your Azure Service Principal and Subcription details.
1. Create a docker image with `docker build -t "openshift-azure-utils:dockerfile" .`
1. Now you can run the image and run the command you need, for instance `python add-node.py`. Or you can run an interactive bash console with `docker run -it <image id> /bin/bash` and n