# My Minikube Project -not tested-

## Prerequisites

* Ubuntu 20.04
* [Install Minikube](#install-minikube)

## Install Minikube

```bash
curl -Lo minikube https://storage.googleapis.com/minikube/releases/latest/minikube-linux-amd64 \
  && chmod +x minikube
```

## Start Cluster

```bash
minikube start
```


## Run Application

* Clone this repository
```bash
git clone https://github.com/timeazsk/my-docker-project.git
```

* Change directory
```bash
cd my-minikube-project
```

* Create Resources
```bash
kubectl apply -f ./liferayapp.yaml
kubectl apply -f ./mysql-config.yaml
kubectl apply -f ./mysql-pv.yaml
kubectl apply -f ./mysql-secret.yaml
kubectl apply -f ./mysql.yaml
kubectl apply -f ./nginx.yaml
```


 > Application is started on http://localhost:30081 \
 > Default credentials are `adminuser:adminpassword` 
