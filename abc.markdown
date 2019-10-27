# About Pod

Created: Oct 27, 2019 1:30 PM
Last Edited By: Wonsik Ha
Last Edited Time: Oct 27, 2019 1:33 PM
Type: Oct 27, 2019 1:33 PM

## Specific Pod`s Full YAML

kubectl get po jordi-4bxm8 -o yaml

## Specific Pod`s Full JSON

kubectl get po jordi-4bxm8 -o json

## Pod`s separate Fields Information

kubectl explain pods

## Pod`s detailed fields Information

kubectl explain pod.spec

## Examples of YAML file.

    apiVersion: v1
    kind: Pod
    metadata:
    	name: kubia-manual
    spec:
    containers:
    image: bearstark/jordi
    name: jordi
    ports:
    containerPort: 8080
    protocol: TCP

- 

## Create a Pods using YAML.

kubectl create -f <yaml file dir.>

## Check a specific Pod`s Log

`kubectl logs <pod`s id>`

`kubectl logs <pods id> -c <containers id>`

## When a request is received, a command about turning over toward specific ports.

kubectl port-forwarding <pod`s id> <received port number>:-[
