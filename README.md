# k8s-nginx


kubectl run my-nginx --image=nginx --replicas=1 --port=80

kubectl get deployment -o wide

kubectl get pods -o wide



service:
 kubectl expose deployment my-nginx --port=80 --type=LoadBalancer
 kubectl get service -o wide
 
