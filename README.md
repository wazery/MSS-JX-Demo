# MSS Jenkins X Demo 

Example Jenkins X application based on [@jstrachan devoxxrocks app](https://github.com/jstrachan/devoxxrocks)

# Installation of Required Tools

* [Kubectl](https://kubernetes.io/docs/tasks/tools/install-kubectl/)
* [JX](https://jenkins-x.io/docs/getting-started/setup/install/)

# Creating EKS Cluster

```
jx create cluster eks --region eu-central-1 \
 --cluster-name jxdemoo \
 --default-environment-prefix jxdemo \
 --node-type c5.2xlarge \
 --nodes 1 \
 --nodes-max 1 \
 --nodes-min 1 \
 --node-volume-size 100
```
 
# Installing Jenkins X platform on the cluster

`jx boot`
