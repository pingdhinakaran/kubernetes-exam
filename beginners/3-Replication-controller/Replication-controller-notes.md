Controllers are the brains behind the kubernetes.

They are the processes that monitor Kubernetes objectes and respond accordingly 

In this section we are going to see one controller 

                    Replication Controller
                    -----------------------

So what is replica , whay do we need a replication controller?

 The replication controller helps us run multiple instances of a single pod in the kubernetes cluster, This providing high availability. 

 so does that mean , you can't use a replication controller if you plan to have a single pod ?  

 No 

 Even if you have a single pod, the replication controller can help by automatically bringing up a new. replica: 1 

 Does the replication controller ensures that the specified number of pods are running at all times, even its just one or 100 pods. 

And another reson we need replication controller:
-------------------------------------------------

* Load balancing & scaling 

Replication controller is to create multiple pods to share the load across containers. 


Replication controller and ( vs ) Replica set :
------------------------------------------------

* Its important to note that, there are two similar terms replication controller and replicas set.

* But have the same purpose, but they are not the same.

* Replication controller is old the older technolgy, That is being replaced by replicas set properly.

#### Replicaset is the new Recommended way to set up replication

Replica set, also termed as rs in short, is almost same as the replication controller is, only with a single difference. The replica set are also known as next generation replication controller. The only difference between replica set and replication controller is the selector types.

The replication controller supports equality based selectors whereas the replica set supports equality based as well as set based selectors.




