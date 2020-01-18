# kubix-cli
These are cli tools to administer Kubix

1. klogin

klogin is  to get the kube config file. At the back, this will call pks get-kubeconfig. Sample usage:-
```
klogin username clustername
``` 

klogin can also be use to login directly to the desired namespace. At the back, this will call pks get-kubeconfig and kubectl config set-context. Samplage usage:-
```
klogin username clustername namespacename
```


2. kmenu

kmenu is tool to select the available namespaces in the cluster. A prerequisite for kmenu is kube config file which can be obtained by using klogin or pks get-kubeconfig. After the prerequisite is met you can simply issue the command kmenu and all avilable namespaces will be shown with a number. Select the number to go to the desired namespace. At the back, this will call kubectl config set-context


