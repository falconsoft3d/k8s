# k8s

# 01 - Wordpress
````
git clone https://github.com/falconsoft3d/k8s.git
cd k8s
cd 01-wordpress
kubectl apply -f 00-namespace.yaml
kubectl get ns
kubectl -n testing apply -f 01-wordpress-service.yaml
kubectl -n testing get svc
kubectl -n testing apply -f 02-wordpress-rc.yaml
kubectl -n testing get pods
kubectl -n testing delete pod wordpress-j7cxt
kubectl get nodes -o wide
kubectl delete namespace testing 
````
