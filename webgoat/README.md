Run OWASP Webgoat on a Kubernetes cluster. 

This will not persist any data on re-launch. 

Always use common sense when running intentionally vulnerable applications on your infrastructure. Do not open to the internet. 

Launch the Webgoat deployment:
`kubectl create -f webgoat-deployment.yaml`