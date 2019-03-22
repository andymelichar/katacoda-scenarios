With Rancher, you can initialise multiple clusters with one single central place to manage them. The Rancher control plane is deployed as a Docker Container.

## Task

To start Rancher, run the command:

`docker run -d -p 443:443 --name=rancher rancher/rancher:v2.0.2`{{execute}}

Once started, you can view the Rancher dashboard at https://[[HOST_SUBDOMAIN]]-443-[[KATACODA_HOST]].environments.katacoda.com

Rancher may take one or two minutes to start. You can view the boot process with `docker logs rancher`{{execute}}

## Create User
Once started, the first step is to configure a password for the login admin of the cluster. For a random password, have Rancher generate the password for you.

## Confirm Server URL

Once the password is created, confirm the URL for the cluster.

<img src="/courses/rancher/deploy-kubernetes-cluster-with-rancher/server-url.png" />

Rancher is now running!! In the next step, in the next step you'll use this cluster to configure Kubernetes.
