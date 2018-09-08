# k8s-nginx


kubectl run my-nginx --image=nginx --replicas=1 --port=80

kubectl get deployment -o wide

kubectl get pods -o wide



service:


 kubectl expose deployment my-nginx --port=80 --type=LoadBalancer
 
 
 
 
 kubectl get service -o wide
 


yaml:

    
   kubectl apply -f nginx.yaml
   
   
   
   
 nodes:
 
  kubectl get nodes
  
  label:
  
  kubectl label nodes <node name> node=app
 
 
 
 node selector:
  ---------
 spec:
      containers:
      - name: my-nginx
        image: nginx
        ports:
        - containerPort: 80
        nodeSelector:
         node: app
----



kuebctl apply -f nginx.yaml



kubectl get pods -o wide
