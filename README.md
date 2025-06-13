# cicd-nginx delivery pipeline using Google Cloud Build and Google Cloud Deploy

# Steps below are dependent on the successful completion of https://github.com/Yougo007/gke-cluster


Step 1: Fork or clone git repo https://github.com/Yougo007/cicd-nginx.git ..


Step 2: Grant the N-computer@developer.gserviceaccount.com in dev, uat & prod permission to container registry in the delivery-pipeline project...


Step 3: Grant the N-computer@developer.gserviceaccount.com from the delivery-pipeline project, Kubernetes Engine Developer role access in dev, uat & prod projects


Step 4: Create and run a cicd-nginx pipeline build trigger in cloud build. (This can also be done using terraform as part of IaC).


Step 5: Promote build from dev-to-uat-to-prod. This is done by clicking promote and deploy.

You can require approval for any target, and you can approve or reject releases into that target. Approvals can be managed programmatically by integrating your workflow management system (such as ServiceNow), or other system, with Google Cloud Deploy using Pub/Sub and the Google Cloud Deploy API.
To require approval on any target, set requireApproval to true in the target configuration:
