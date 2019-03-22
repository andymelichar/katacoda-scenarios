The next step is to deploy Kubernetes, in this case, we'll start by configuring a single node instance of Kubernetes.

## Add Our Node to the Cluster

Switch to the **Cluster Node** tab on the right, and paste the command you copied from the Rancher UI in the previous step. Press **Enter** on your keyboard to execute the command.

At this point the node will pull down the required docker images, will register with Rancher and the Kubernetes cluster, and will configure itself to serve all of the roles we selected in the previous step.

## Watching the Node Build

After the node pulls down and runs the initial agent docker image, if you switch back to the **Rancher** tab, you should see a message "1 new node has registered" below the command you copied in the previous step. Our node is now registered with Rancher and Kubernetes, and is building itself up to become part of the cluster.

Click **Done** at the Add Cluster screen, which will return you to a list of clusters in Rancher.

The process of building up a node can take several minutes. During this time you'll see the state of the cluster is set to **Provisioning** - you may see some errors during this process, don't be alarmed. Many new services are being installed on the node during the build. Kubernetes will try to run commands multiple times while waiting for the services to become active.

Once the node is done building itself, you should see the state of the cluster switch from **Provisioning** to **Active**. At this point the node is done building and the cluster is ready for us to put to work!

**Next we will deploy an application to our cluster.**
