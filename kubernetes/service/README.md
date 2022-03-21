# Services
Just as the kubectl run command is an easy way to create a Kubernetes deployment, we can use kubectl expose to create a service. Let’s create some deployments and services so we can see how they work:
```sh
kubectl run alpaca-prod \
  --image=gcr.io/kuar-demo/kuard-amd64:blue \
  --replicas=3 \
  --port=8080 \
  --labels="ver=1,app=alpaca,env=prod"
  
kubectl expose deployment alpaca-prod

kubectl run bandicoot-prod \
  --image=gcr.io/kuar-demo/kuard-amd64:green \
  --replicas=2 \
  --port=8080 \
  --labels="ver=2,app=bandicoot,env=prod"
  
kubectl expose deployment bandicoot-prod

```
```sh
kubectl get services -o wide
NAME             CLUSTER-IP    ... PORT(S)  ... SELECTOR
alpaca-prod      10.115.245.13 ... 8080/TCP ... app=alpaca,env=prod,ver=1
bandicoot-prod   10.115.242.3  ... 8080/TCP ... app=bandicoot,env=prod,ver=2
kubernetes       10.115.240.1  ... 443/TCP  ... <none>
```
