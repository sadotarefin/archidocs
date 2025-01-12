# Deploy WordPress on Minikube with Port Forwarding
## Prerequisites
- Minikube installed and running.
- Docker installed on your system.
- `kubectl` command-line tool configured to use Minikube.

## 1. Start Minikube
minikube start --driver=docker

## 2. Create the MariaDB Deployment File
- Refer to mariadb.yaml File
- Run 'kubectl apply -f mariadb.yaml'

## 3. Create the WordPress Deployment File
- Refer to wordpress.yaml File
- Run 'kubectl apply -f wordpress.yaml'

## 4. Verify Deployments
- kubectl get pods

## 5. Port Forward the WordPress Service
- kubectl port-forward service/wordpress 8080:80

## 6. Access WordPress
- Browse http://localhost:8080


## 7. Stop Port Forwarding
To stop the port forwarding, press Ctrl+C in the terminal running the kubectl port-forward command.

## 8. Cleanup (Optional)
- kubectl delete -f wordpress.yaml
- kubectl delete -f mariadb.yaml
