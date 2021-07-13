## PODS OVERVIEW:

#### Pods are the smallest deployable units of computing that you can create and manage in Kubernetes. A Pod is a group of one or more containers, with shared storage and network resources, and a specification for how to run the containers. 
#### Pod wraps with either one running container or multiple running cotainer.

## To spin a container inside a pod: 
`kubectl apply -f nginx-pod.yml`


## To spin multiple container inside a pod
`kubectl apply -f multi-pod.yml`