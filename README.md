# springboot_study

### preparations
<ul>jdk</<ul>
<ul>gradle</<ul>
<ul>docker</<ul>
<ul>kubenetes</<ul>
<ul>kubectl</<ul>
<ul>istioctl</<ul>
<ul>eksctl</<ul>
<ul>awscli</<ul>
<ul>fluxctl</<ul>

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