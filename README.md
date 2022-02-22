# nginx-with-data-persistence-on-kubernetes
Deploy Nginx on Kubernetes with Data Persistence 

Step 01
_______
Follwing Files Included.

index.html  
nginx-deployment.yaml 

Step02
_______
Create configmap , name my-htmlfile by running Following Command

kubectl create configmap my-htmlfile --from-file=./index.html

Step03
_______
Apply the nginx deployment by running the following Command

kubectl apply -f nginx-deployment.html

Step04
_______
Expose the Deployment as a LoadBalancer service by running following Command

kubectl apply -f nginx-deployment.html

Step05
_______
Check the Pods and Public IP by Running Following Command

kubectl get pod
