# cluster-config
Configuration for k8s cluster


## Create and push master and slave images
docker build -f master.Dockerfile -t michalleszczynski/jenkins-master .
docker push michalleszczynski/jenkins-master

docker build -f slave.Dockerfile -t michalleszczynski/jenkins-slave-jnlp .
docker push michalleszczynski/jenkins-slave-jnlp

