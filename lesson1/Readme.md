minikube start 
cd app/ConsoleApp7
docker build -t <вашлогин на docker.hub.com>/testapp .
docker push
kubectl apply -f deployment.yaml
kubectl apply -f service.yaml