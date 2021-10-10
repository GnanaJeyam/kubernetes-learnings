## <b>Volume Type -> emptyDir 

1. It is created during the pod creation and it can be accessed by containers once it is mounted.
2. Help with sharing data across containers.
3. volume and volumemount should share the same name.

<br>

## To spin up multiple containers inside a pod:
    
    `kubectl apply -f emptyDir-volume.yml`

## To Navigate into the nginx container:

    `kubectl exec -it empty-dir-volume -c nginx sh`

## To Navigate into the busybox container:

    `kubectl exec -it empty-dir-volume -c busybox sh`