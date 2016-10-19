## Scumblr with a persistant Mysql database

### Requirements
10GB Volume on Google Compute

### Instructions
1. Deploy your secrets:
`kubectl create -f scumblr-secrets.yaml`
2. Create a Persistent Volume:
`kubectl create -f gce-volumes.yaml`
3. Launch the Mysql deployment:
`kubectl create -f scumblr-deployment`
4. Launch the Threadfix deployment:
`kubectl create -f scumblr-deployment.yaml`