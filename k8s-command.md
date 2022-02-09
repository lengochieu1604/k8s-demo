#kubectl apply commands in order

kubectl apply -f mongo-secret.yaml
kubectl apply -f mongo-deployment.yaml
kubectl apply -f mongo-configmap.yaml 
kubectl apply -f mongo-express-deployment.yaml

#kubectl get commands

kubectl get pod
kubectl get pod --watch
kubectl get pod -o wide
kubectl get service
kubectl get secret
kubectl get all | grep mongodb

#kubectl debugging commands

kubectl describe pod mongodb-deployment-xxxxxx
kubectl describe service mongodb-express-service 
kubectl logs mongodb-express-xxxxxx

#give a URL to external service in minikube

minikube service mongo-express-service