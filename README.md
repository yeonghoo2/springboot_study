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

<ol>create eks cluster</ol>
```bash
eksctl create cluster -f cluster.yaml
```
<ol>create eks managed worker node</ol>
<ol>create namespace & istio injection</ol>
<ol>install istio (create ingress gateway)</ol>
```bash
istioctl manifest generate > manifest.yaml
# set up annotation in service
kubectl apply -f manifest.yaml
```
<ol>(optional) create internal ingress gateway</ol>
```bash
istioctl install -f internal.yaml
```
<ol>apply yaml</ol>

<ol>start springboot with springboot initializer</ol>

namespace : devops
docker image local