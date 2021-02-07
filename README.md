# springboot_study

### preparations
<uo>
jdk
gradle
docker
kubenetes
kubectl
istioctl
eksctl
awscli
fluxctl
</uo>

<uo>create eks cluster</uo>
```bash
eksctl create cluster -f cluster.yaml
```
<uo>create eks managed worker node</uo>
<uo>create namespace & istio injection</uo>
<uo>install istio (create ingress gateway)</uo>
```bash
istioctl manifest generate > manifest.yaml
# set up annotation in service
kubectl apply -f manifest.yaml
```
<uo>(optional) create internal ingress gateway</uo>
```bash
istioctl install -f internal.yaml
```
<uo>apply yaml</uo>

<uo>start springboot with springboot initializer</uo>

namespace : devops
docker image local