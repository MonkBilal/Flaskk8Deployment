## Project Summary

This is a very basic implementation of Flask app Deployment on a kubernetes cluster.It contains a Deployment.yaml file which contains two kubernetes resources one is 
Deployment itself another is a NodePort Service which is exposing the application on a particular port.

## Requirements

* A kubernetes cluster (Minikube)
* Docker engine
* Dockerhub Repository

## Running Deployment on k8 Cluster

To run the Deployment:

$ kubectl apply -f Deployment.yaml 

## Access the application

To access the running application you can use your minikube ip:

http://\<your-minikube-ip\>:30002
