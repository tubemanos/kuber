# kuber

build docker 

    docker build -t alxst/flaskapp:flask .

push to dockerhub

    docker push -t alxst/flaskapp:flask


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



Useful links:

https://rtfm.co.ua/kubernetes-zapusk-gravl-v-minikube/

https://habr.com/ru/company/flant/blog/333470/

https://kubernetes.io/ru/docs/reference/kubectl/cheatsheet/

https://eax.me/kubernetes/





