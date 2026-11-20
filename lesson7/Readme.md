Кратко:
1. helm uninstall app
2. установить argocd
kubectl create namespace argocd
kubectl apply -n argocd --server-side --force-conflicts -f https://raw.githubusercontent.com/argoproj/argo-cd/stable/manifests/install.yaml
kubectl patch svc argocd-server -n argocd -p "{\"spec\": {\"type\": \"LoadBalancer\"}}"
3. получить ip-адрес kubectl get svc argocd-server -n argocd -o=jsonpath='{.status.loadBalancer.ingress[0].ip}'
4. получить пароль kubectl get secret argocd-initial-admin-secret -n argocd -o jsonpath='{.data.password}' | base64 -d
5. Поменять docker.yaml

Полно: 
https://teletype.in/@olegtar/editor/K4Th1Atgz2N
