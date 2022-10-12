# ReplicaSet Worksheet:

__Task 1, step 7: Enter the command you used for scaling the replica set:__
```
kubectl scale --replicas=3 rs/nginx-replica

__Task 1, step 9: What happened after applying another pod with matching selectors as the ReplicaSet?__
```
It deleted an existing pod to keep the deployment at 3
Normal  SuccessfulDelete  114s (x2 over 5m18s)  replicaset-controller  Deleted pod: nginx-pod
