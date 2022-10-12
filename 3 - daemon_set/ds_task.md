# DaemonSet Worksheet


__Task 4, step 5: Once you apply the DaemonSet, what happens and why?__

```
It created a daemonset with the name nginx with the nodeType=health
```

__Task 4, step 7: What happened when you labeled the node and why?__

```
kubectl label node minikube nodeType=healt
node/minikube not labeled

The label was already applyed by the daemonset.