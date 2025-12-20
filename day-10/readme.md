Namespaces
In Kubernetes, a namespace is a way to logically divide a cluster into multiple virtual clusters. It helps organize and isolate resources (like Pods, Services, Deployments) so teams, projects, or environments don’t conflict with A B each other.




kubectl create namespace demo
kubectl create deploy nginx-demo --image=nginx -n demo
kubectl get pods nginx-demo-98d9dcdf8-98hqg -o wide -n demo
kubectl exec -it nginx-demo-98d9dcdf8-98hqg -n demo -- sh
kubectl delete deployment nginx-deploy
kubectl scale deployment nginx-demo --replicas=3 -n demo

