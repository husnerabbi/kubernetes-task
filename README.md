# task-kubernetes

Node Web App.
========
NodeJS simple web server application.


Prerequisites:

* minikube is running.
* git
* check status by command.
```bash
minikube status
```
## out put look like this
`minikube: Running`
`cluster: Running`


## Run App on Kubernets (minikube) environmnet.
```bash
Clone below mentioned repository on your minikube host, cd into kubernetes-task directory.
git clone https://github.com/husnerabbi/kubernetes-task.git
cd kubernetes-task

Run below mentiond command.
kubectl create -f deployment.yaml
kubectl create -f service.yaml

=========
check the status
kubectl get pods

```

## Test App:
```bash
* check the minikube ip.
minikube ip

Now you can access application * Url: `http://<minikube-ip>:31000`
or `curl http://192.168.42.13:31000` replace IP 192.168.42.13 with your minkube IP.
* Reult will be.
`Server responded with success !! `

## Note we run the application 31000 port because the default minikube port range is 30000-32767.
