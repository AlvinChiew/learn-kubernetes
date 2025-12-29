# Learn Kubernetes

## Quick Start

1. `brew install minikube`

   - Minikube is used to host master and node on local machine for testing purposes.

2. `minikube start --driver docker`

   - start Minikube inside docker container

3. `minikube status` , `kubectl get node`, `kubectl get pod`

   - status check

4. `kubectl apply -f mongo-config.yaml`, `kubectl apply -f mongo-secret.yaml`, `kubectl apply -f mongo.yaml`

   - create mongo config, secret, deployment & service

5. `kubectl apply -f webapp.yaml`

   - create webapp deployment & service

6. `minikube service webapp-service`

   - serve webapp on minikube

7. `kubectl get all`, `kubectl get config map`, `kubectl get secret`, `kubectl describe service webapp-service`, `kubectl describe pod webapp-deployment-768fbb8d95-kp2ht`, `kubectl logs webapp-deployment-768fbb8d95-kp2ht -f`

   - more status check

8. `kubectl get svc`, `minikube ip`

   - check service port and ip

9. `kubectl delete secret my_secret`

   - delete secret

10. `kubectl delete all --all`

    - delete all resources

11. `kubectl drain minikube --ignore-daemonsets --delete-local-data --force`, `kubectl delete node minikube`, `minikube stop`
    - decommission minikube

## Extra

1. `echo -n <text> | base64`
   - convert text to base64
