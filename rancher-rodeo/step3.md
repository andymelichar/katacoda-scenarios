The next step is to deploy Kubernetes, in this case, we'll start by configuring a single node instance of Kubernetes.

A single node instance has etcd, the Kubernetes Control Plane and a Kubernetes node to all run on the same machine. Within production this would be deployment onto multiple nodes, however, a single node is great starting place for testing and experimenting.

## Configuring Node Role

By ticking the etcd and control plane boxes, the command to initialise the cluster at the top will change. This command will deploy the correct configuration for our single node cluster.

## Deploy Node 

When you're happy with the configuration, run the command in the Katacoda Terminal window. Note, Rancher have a helpful "Copy to Clipboard" button to make this easier.

After running the command, the Rancher dashboard should report **1 new node has registered**. Rancher will now initalize the Kubernetes cluster.

Click **Done** to view the progress of the deployment.
