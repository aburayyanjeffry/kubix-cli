# kubix-cli
These are cli tools to administer Kubix

1. klogin
klogin is use to get the kube config files so that user can . At the back, this will call pks get-kubeconfig. Sample usage:-
```
klogin username clustername
``` 

klogin can also be use to login directly to the desired namespace. At the back, this will call pks get-kubeconfig and kubectl config set-context. Samplage usgage:-
```
klogin username clustername namespacename
```
