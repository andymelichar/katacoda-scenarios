Rancher is now starting all the components of Kubernetes. This will take a couple of minutes. Afterwards you will have a fully functional Kubernetes cluster.

Within the UI, you can select the newly deployed Cluster to view the details, usage and status.

In the corner of the details page, you can select **Launch Kubectl**. This provides you with an interface to manage and control your cluster.

Try running `kubectl get nodes`{{copy}} to see the nodes available in the cluster.

 You should see a single v1.10.1 node as ready. You now have a running Kubernetes cluster managed by Rancher.