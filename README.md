# EFK Stack on Kubernetes

You can use your kubernetes environment. I would suggest you use 4 CPUs and 4GB of RAM per node with 1 Master and 2 Worker or more.

Run these manifests one by one.
```
kubectl create -f [manifest-name].yaml
```

To access kibana use `kubectl port-forward [kibana-podname] 5601:5601 -n kube-logging`.
