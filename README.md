# kuber

build docker 

    docker build -t alxst/flaskapp:tagname:flask .

push to dockerhub

    docker build -t alxst/flaskapp:tagname:flask

docker run from dockerhub

    docker run --rm --name web -p 8080:8080 alxst/flaskapp:flask


Run background docker from dockerhub

    docker run --rm --name web -p 8080:8080 alxst/flaskapp:flask

stop docker

    docker stop web



Kuberneties

Get the list of the nodes and podes

    kubectl get nodes
    kubectl get pods -o wide

Delete particular pode

    kubectl delete pod <podname>

Create deployment

    kubectl create -f flask.yml

Check it

    kubectl get deployments

Starting the service

    kubectl expose deployment flaskapp --type=NodePort

Checking

    kubectl get services

Get the URL

    minikube service flaskapp --url






