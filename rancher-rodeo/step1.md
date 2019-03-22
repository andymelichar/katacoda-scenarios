With Rancher, you can initialize multiple clusters with one single central place to manage them. In production, Rancher would typically be ran in its own highly-available kubernetes cluster. For purposes of this tutorial, we'll be running Rancher in a Docker Container.

## Start an Instance of Rancher

To start Rancher, run the command:

`docker run -d -p 443:443 --name=rancher rancher/rancher:latest`{{execute}}

Rancher may take one or two minutes to start. You can view the boot process with `docker logs rancher`{{execute}}

Once started, you can view the Rancher dashboard at <a href="https://[[HOST_SUBDOMAIN]]-443-[[KATACODA_HOST]].environments.katacoda.com" target='_blank'>https://[[HOST_SUBDOMAIN]]-443-[[KATACODA_HOST]].environments.katacoda.com</a> - this link will show a blank page until the Rancher server finishes booting up. Once it is booted you can continue to the next step.

## Confirm Server URL

Once Rancher has started, the first task is to confirm our server URL. You can leave the URL set to the default value and click `Save URL`

**Note:** Depending on how many times/when you refresh, this Server URL confirmation may not display. In that case, continue to the next task.

## Set the Admin Password
Next, we need to configura a password for the Rancher admin user. For a random password, have Rancher generate the password for you. Otherwise enter your desired password in both fields and click `Save`

**Notes:** Depending on how many times/when you refresh, this password set page may ask for your current password. If this happens, enter `admin` as the current password.

Rancher is now running!! In the next step, we will add a cluster for Rancher to manage.