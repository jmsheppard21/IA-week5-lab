# StatefulSet Worksheet

__Task 5, step 3: Describe what happened and what you noticed about the pods and the volumes for them.__

```
 These were created
 Pods -  stateful-nginx-0, stateful-nginx-1, and stateful-nginx-2.
 Volumes - persistentvolumeclaim/html-stateful-nginx-0, ersistentvolumeclaim/html-stateful-nginx-1
           persistentvolumeclaim/html-stateful-nginx-2
           persistentvolume/pvc-367bab66-4359-414d-920e-154b85095e99
           persistentvolume/pvc-42f50a67-bf06-44ee-80c6-b6dbcdaf5bb4
           persistentvolume/pvc-626d77ef-8e52-4974-92eb-6c55693d330d 

__Task 5, step 4: Did anything change? Why or why not?__

```
Nothing changed as the updateStrategy is set to OnDelete.
```

__Task 5, step 6: What happened and why?__

```
the app version for pod stateful-nginx-0  changed to version 2 as it was delete and recreated. 
```

__Task 5, step 9: What happens this time?__

```
all 3 pods upated to app version 3.0
```

__Task 5, step 11: Repeat step 10. Was everything deleted? Why or why not?__

```
No the storage volumes were not deleted as they were persistent
```