# Add a node to your Openshift cluster

This util allows you to scale your cluster up. You need to provide the characteristics for your cluster.

## Proposed things to work on

1. Create script to set up VM with network configuration
1. Create script to call ansible script to add Node to cluster
1. Set up a dockerfile ready to use the libraries and tools for python on Azure
1. Publish docker image to deploy as a pod inside the Openshift that can manage the new pool of nodes.
