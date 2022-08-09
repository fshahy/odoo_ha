minikube start -p mycluster
minikube dashboard -p mycluster
minikube tunnel -p mycluster

kubectl create -f postgres-configmap.yaml
kubectl create -f postgres-storage.yaml
kubectl create -f postgres-deployment.yaml

kubectl create -f odoo15-storage.yml
kubectl create -f odoo15-deplyment.yaml
