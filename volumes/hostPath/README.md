## <b>Volume Type -> hostPath 

1. Here the data is actually stored in Node and not in pod. So if pod dies no problem we can retrieve the data until the node is available. If the pod is scheduled in a new node then we can't retrieve the data.

2. hostPath volume mounts a file or directory from the host node’s filesystem into your Pod.

3. Data is not available if node is down due to some failure.

<br>

## hostPath contains multiple types:

    The most commonly used types are `Directory` and `File`.


### <b>Note</b>: Before applying the yaml files make sure you create the required file or directory in the Worker Node

<br>

## hostPath with Directory type:

    `kubectl apply -f hostPath-directory.yml`

## hostPath with File type:

    `kubectl apply -f hostPath-file.yml`

## To Navigate into the nginx container:

`kubectl exec -it hostpath-file -c nginx sh`

## To Navigate into the busybox container:

`kubectl exec -it hostpath-file -c busybox sh`