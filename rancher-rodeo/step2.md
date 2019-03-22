Rancher can manage and deploy Kubernetes on a cloud provider such as AWS, or it can manage self-hosted/on-premise clusters. For this tutorial we'll be setting up a self-hosted cluster.

## Add a Cluster

To begin the installation, click the **Add Cluster** button and select the cluster type of **Custom**.

Provide a friendly name for the cluster, such as `my-kubernetes-cluster`{{copy}} and enter it in the **Cluster Name** field. Then click **Next**.


## About Node Roles

Rancher is going to provide us with a command to run on our nodes, which will have them join our new cluster. In order to do that, we need to tell Rancher what roles want the new nodes to have.

### etcd
etcd is the main data store for Kubernetes configuration. Nodes with the etcd role will store and replicate a copy of the etcd database.

### Control Plane
The Control plan is the workhorse of the Kubernetes cluster. It performs necessary tasks to keep the cluster functional. Nodes with the Control Plane roll will help maintain the cluster by running these necessary tasks.

### Worker
The Worker role tells Kubernetes which nodes should be able to receive deployments. Nodes with the Worker role will host the resources that we add in Rancher.

## Select Node Roles and Copy the command

We'll only be setting up one node for this tutorial, so we want that node to have all of the roles necessary to run a cluster. Check the boxes next to **etcd**, **Control Plane**, and **Worker**.

Next, click the Clipboard icon next to the command that is displayed at the bottom of the page. This will copy the command to your clipboard for use in the next step.

***Next we will add a node to our cluster.***
