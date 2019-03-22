The next step is to deploy Kubernetes, in this case, we'll start by configuring a single node instance of Kubernetes.

A single node instance has etcd, the Kubernetes Control Plane and a Kubernetes node to all run on the same machine. Within production this would be deployment onto multiple nodes, however, a single node is great starting place for testing and experimenting.

## Add Our Node to the Cluster

Switch to the **Cluster Node** tab on the right, and paste the command you copied from the Rancher UI in the previous step. Press **Enter** on your keyboard to execute the command.

At this point the node will pull down the required docker images, will register with Rancher and the Kubernetes cluster, and will configure itself to serve all of the roles we selected in the previous step.

## Watching the Node Build

Switch back to the Rancher tab
