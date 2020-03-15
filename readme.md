 # Usage
 
1 Deploy the PV and PVC of the YAML file:

				kubectl apply -f mysql-pvol.yaml



2 Deploy the contents of the YAML file:

				kubectl apply -f mysql-deployment.yaml
				
				
3 Run on kubernetes 

		kubectl get pods -l app=mysql
		kubectl get deployments
		kubectl describe deployment mysql
		kubectl get svc
		kubectl describe pvc mysql-pv-claim
		kubectl run -it --rm --image=mysql:5.6 --restart=Never mysql-client -- mysql -h mysql -ppassword
