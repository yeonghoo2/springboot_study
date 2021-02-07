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
1. create eks cluster
```bash
eksctl create cluster -f cluster.yaml
```
2. create eks managed worker node
3. create namespace & istio injection
4. install istio (create ingress gateway)
```bash
istioctl manifest generate > manifest.yaml
# set up annotation in service
kubectl apply -f manifest.yaml
```
5. (optional) create internal ingress gateway
```bash
istioctl install -f internal.yaml
```
6. apply yaml

7. start springboot with springboot initializer

namespace : devops
docker image local