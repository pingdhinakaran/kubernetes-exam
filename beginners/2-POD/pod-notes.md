* Kubernetes uses YAML files as input for pod, deployement, service...etc 

All these follows similler structure: 

```
apiVersion:

Kind:

metadata:





Spec:

```
Kubernetes defenition files always contains 4 top level fileds. 

These are top level or root level properties. 

And this also a required fileds so its must be in our configurtion. 


apiVersion: 
=========== 

This is the version of the Kubernetes API, you are using to create the objects. 

Depending on what we are trying to create we must use the right API version. 

For now since we are working on pods, so we will set the API version as we want.

| Kind         | Version     |
|--------------|----------   |
| POD          | v1          |
| Service      | v1          |
| ReplicaSet   | apps/v1     |
|  Deployement | Deployement |


### Kind :
======

The Kind refers to type of object we are trying to create which in this case happens to be pod.

so we will set as POD. 

some other possible values here could be ReplicaSet or Deployement or service 
which is what you see in the above table.

Metadata:
=========

The metadata is data, about the object like its name and labels etc. 
As you can see unlike the first two where you have specified string value ( apiVersion, kind )

```
apiVersion: v1          ---------- String

kind: Pod               ---------- String

metadata:
   name: myapp-pod
   labels:                       --------- Dictionary
     app: myapp

spec:

```

Spec: 
=====

Depending on the object we are going to create, This is where we would provide additional 
information to kubernetes pertaining to that object.

This is going to be different for different objects so its important to understand 
OR refer to the documentation section to get the right format for each.
 
since we are only creating a pod with a single container in it, Its easy . spec is a dictionary. 

```
spec:
  containers:
    - name: nginx-continer
      image: nginx
```




