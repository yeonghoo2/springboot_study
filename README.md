# springboot_study

### preparations
- jdk
- gradle
- docker
- kubenetes
- kubectl
- istioctl
- eksctl
- awscli
- fluxctl


### action
 + create eks cluster
```bash
eksctl create cluster -f cluster.yaml
```
 + create eks managed worker node
 + create namespace & istio injection
 + install istio (create ingress gateway)
```bash
istioctl manifest generate > manifest.yaml
# set up annotation in service
kubectl apply -f manifest.yaml
```
 + (optional) create internal ingress gateway
```bash
istioctl install -f internal.yaml
```
 + apply yaml

 + start springboot with springboot initializer

namespace : devops
docker image local