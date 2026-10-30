1.kubectl apply -f deploymentA.yaml  
kubectl apply -f deploymentB.yaml  
kubectl apply -f serviceA.yaml  
kubectl apply -f serviceB.yaml  
kubectl apply -f ingressA.yaml  
kubectl apply -f ingressB.yaml  
2. kubectl apply -f https://raw.githubusercontent.com/kubernetes/ingress-nginx/controller-v1.10.1/deploy/static/provider/cloud/deploy.yaml  
3. Дернуть так, и с http-заголовком X-Version: v2  