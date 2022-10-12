# Job and CronJob Worksheet

__Task 6, step 2: How many jobs run? How many run at the same time?__


```
8 jobs run, 2 at the same time. 

NAME                  READY   STATUS      RESTARTS   AGE
pod/batch-app-2jd47   0/1     Completed   0          2m26s
pod/batch-app-49sxz   0/1     Completed   0          2m36s
pod/batch-app-592c6   0/1     Completed   0          2m36s
pod/batch-app-fl8th   0/1     Completed   0          2m31s
pod/batch-app-l8xl8   0/1     Completed   0          2m42s
pod/batch-app-pgn64   0/1     Completed   0          2m31s
pod/batch-app-s497r   0/1     Completed   0          2m26s
pod/batch-app-xfr2n   0/1     Completed   0          2m42s

NAME                  COMPLETIONS   DURATION   AGE
job.batch/batch-app   8/8           21s        2m42s
```

__Task 6, step 5: What you observe when running the CronJob?__

```
pod/cron-app-27759752-7grfm   0/1     Completed   0          107s
pod/cron-app-27759752-gbb6s   0/1     Completed   0          111s
pod/cron-app-27759752-gfb25   0/1     Completed   0          98s
pod/cron-app-27759752-pnk5x   0/1     Completed   0          98s
pod/cron-app-27759752-rqpd8   0/1     Completed   0          102s
pod/cron-app-27759752-rw7tx   0/1     Completed   0          102s
pod/cron-app-27759752-zkdhn   0/1     Completed   0          111s
pod/cron-app-27759752-zs459   0/1     Completed   0          107s
pod/cron-app-27759753-2xdmd   0/1     Completed   0          43s
pod/cron-app-27759753-4m9zd   0/1     Completed   0          43s
pod/cron-app-27759753-9lrpn   0/1     Completed   0          51s
pod/cron-app-27759753-ml2ln   0/1     Completed   0          47s
pod/cron-app-27759753-nwkl4   0/1     Completed   0          46s
pod/cron-app-27759753-ttdwz   0/1     Completed   0          40s
pod/cron-app-27759753-wrjj5   0/1     Completed   0          51s
pod/cron-app-27759753-zmbzg   0/1     Completed   0          38s

NAME                     SCHEDULE    SUSPEND   ACTIVE   LAST SCHEDULE   AGE
cronjob.batch/cron-app   * * * * *   False     0        51s             18m

```