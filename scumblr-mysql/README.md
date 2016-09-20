Run Scumblr with a persistant Mysql database

This requires a 10GB Volume on Google Compute!

Deploy your secrets:
`kubectl create -f scumblr-secrets.yaml`

Create a Persistent Volume:
`kubectl create -f gce-volumes.yaml`

Launch the Mysql deployment:
`kubectl create -f scumblr-deployment`

Launch the Threadfix deployment:
`kubectl create -f scumblr-deployment.yaml`