# kuber

build docker 

    docker build -t alxst/flaskapp:tagname:flask .

push to dockerhub

    docker build -t alxst/flaskapp:tagname:flask

docker run from dockerhub

    docker run --rm --name web -p 8080:8080 alxst/flaskapp:flask


