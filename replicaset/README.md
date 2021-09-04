## ReplicaSet OVERVIEW:

#### A ReplicaSet's purpose is to maintain a stable set of replica Pods running at any given time. As such, it is often used to guarantee the availability of a specified number of identical Pods.


## The below command will spin up a 3 replicas of dobby pod: 
`kubectl apply -f replicaset-example.yml`


## To hit the dobby /health Url:
`curl -i <pod-ip>:4444/health`
### Make sure you are inside the cluster to access the running pods.
