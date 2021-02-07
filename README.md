# springboot_study

### preparations
<ol>
jdk
gradle
docker
kubenetes
kubectl
istioctl
eksctl
awscli
fluxctl
</ol>

<ul>create eks cluster</ul>
```bash
eksctl create cluster -f cluster.yaml
```
<ul>create eks managed worker node</ul>
<ul>create namespace & istio injection</ul>
<ul>install istio (create ingress gateway)</ul>
```bash
istioctl manifest generate > manifest.yaml
# set up annotation in service
kubectl apply -f manifest.yaml
```
<ul>(optional) create internal ingress gateway</ul>
```bash
istioctl install -f internal.yaml
```
<ul>apply yaml</ul>

<ul>start springboot with springboot initializer</ul>

namespace : devops
docker image local