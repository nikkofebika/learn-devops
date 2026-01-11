kubectl create -f filename.yml

# all
kubectl get all
kubectl get all --namespace namespaceName

kubectl delete all --all
kubectl delete all --all --namespace namespaceName

# node
kubectl get nodes/node/no -o wide
kubectl describe node nodeName
kubectl label node nodeName key=value --overwrite

# pod
kubectl get pods -o wide
kubectl describe pod podName

kubectl delete pod podName1 podName2 podName3
kubectl delete pod -l key=value
kubectl delete pod --all --namespace namespaceName

kubectl port-forward podName portAccess:portPod

kubectl label pod podName key=value --overwrite
kubectl get pod --show-labels

kubectl annotate pod podName key=value --overwrite

kubectl get pods --namespace default


# namespace
kubectl get namespaces/ns
kubectl delete namespace namespaceName
kubectl create -f filename --namespace namespaceName

# replicaSet
kubectl get replicaSet/rs
kubectl delete rs rsName

# job
used to run pod once and then terminated it
kubectl get jobs

# service
available type (NodePort, LoadBalancer, ClusterIP, ExternalName)
default type is ClusterIP
kubectl get services

# endpoints
kubectl get endpoints