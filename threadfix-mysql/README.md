Run Threadfix with a persistant Mysql database

This requires a 10GB Volume on Google Compute!

Deploy your secrets:
`kubectl create -f threadfix-secrets.yaml`

Create a Persistent Volume:
`kubectl create -f gce-volumes.yaml`

Launch the Mysql deployment:
`kubectl create -f mysql-deployment`

Launch the Threadfix deployment:
`threadfix-deployment.yaml`

