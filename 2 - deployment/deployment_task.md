# Deployment Worksheet

__Task 2, step 6: After completing step 5 of task 2, what do you notice about the `ReplicaSet` - what is this used for?__
hint: use ` kubectl get rs --show-labels`

```
The lables show the version number.
```

__Task 2, step 7: what command did you use to scale the deployment?__

```
kubectl scale --replicas=4 rs/nginx-deployment-779ddf7fd4
```

__Task 3, step 2: Why are there two replica sets but only one deployment?__

```
It kept the replica set with Verion 1 label
```

__Task 3, step 6: What command did you use to roll back the deployment?__

```
kubectl rollout undo deployment.apps/nginx-deployment --to-revision=1
```
