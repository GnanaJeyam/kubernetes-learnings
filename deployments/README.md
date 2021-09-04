## Deployments Usecase:

### How do you deploy new applications and how do you rollback if something went wrong.?

### Deployments is used for major two reasons 
1. Updates with zero downtime(Rolling updates) 
2. Rollback.

## Job of Deployment:

1. Provides declarative updgrades to Pods using Replicaset.
2. Abstraction on top of replicaset.

## To apply the deployments:

    kubectl apply -f deployment-test.yml


## To view the older history of deployments

    kubectl rollout history deployment/deployment-meta

deployment-meta - Name of the deployment

## To Rollback to the previous versions of Deployment

        kubectl rollout undo deployment/deployment-meta

## To Rollback to the specific revision of Deployment

    kubectl rollout undo deployment/deployment-meta --to-revision=1

During these undo revision process it will try to use older replicaset instead of creating new ones.


## Rolling Update strategy 