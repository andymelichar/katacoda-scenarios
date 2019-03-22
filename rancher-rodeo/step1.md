With Rancher, you can initialize multiple clusters with one single central place to manage them. In production, Rancher would typically be ran in its own highly-available kubernetes cluster. For purposes of this tutorial, we'll be running Rancher in a Docker Container.

## Task

To start Rancher, run the command:

`docker run -d -p 443:443 --name=rancher rancher/rancher:latest`{{execute}}

Rancher may take one or two minutes to start. You can view the boot process with `docker logs rancher`{{execute}}

Once started, you can view the Rancher dashboard at <a href="https://[[HOST_SUBDOMAIN]]-443-[[KATACODA_HOST]].environments.katacoda.com" target='_blank'>https://[[HOST_SUBDOMAIN]]-443-[[KATACODA_HOST]].environments.katacoda.com</a>

You can also click the "Rancher" tab in the right pane of this screen, and click the refresh icon a few times until you see the Rancher splash screen. Then continue to the next step below.

## Confirm Server URL

Once Rancher has started, the first task is to confirm our server URL. You can leave the URL set to the default value and click `Continue`

## Set the Admin Password
Once started, the first step is to configure a password for the login admin of the cluster. For a random password, have Rancher generate the password for you.



Rancher is now running!! In the next step, in the next step you'll use this cluster to configure Kubernetes.
