# EFK Stack on Kubernetes

My environment uses `Ubuntu 16.04` and 4 CPU cores and 4GB of RAM per node.
* 3 master nodes.
* 2 worker nodes.
* 200GB volume attached to worker0 as a Persistent Volume.

Run these manifests one by one.
```
kubectl create -f [manifest-name].yaml
```

To access kibana use `kubectl port-forward [kibana-podname] 5601:5601 -n kube-logging`.
