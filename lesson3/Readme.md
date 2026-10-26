Кратко:

1. Добавить эндпоинт /hc
2. Накатить 
kubectl apply -f blue-deployment.yaml
kubectl apply -f green-deployment.yaml
kubectl apply -f service.yaml
3. Обновить docker.yaml в github/workflow

Полно:
https://teletype.in/@olegtar/GKdXprEbsLh