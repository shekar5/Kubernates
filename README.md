# Kubernates
writting notes from abhishek veeramalla Kubernates videos day wise and Interview and Projects

List :
1. Docker Vs Kubernates --> why need to use kubernates.
2. Architecture of kubernates like control plane and data plane
3. installation and configuration of kubectl,minikube (for practice) and discussion of kops(kubernates installation on real-time) , AKS, EKS, rancher etc..
4.Install first application using pod services and logs and describe command.
5. Kubernates Deployments & Replicasets

Docker vs Pod vs Deployment
Pod also creates the containers like 1 or 2 but doesnt support autohealing but by using deployment we can have replica set which auto heals the pods and re-creates automatically.
 6. Why we need Service (svc) -
 > Load balancing --> In deployment, we have 3 pods but user carries requests to only one pod, but here services Creating multiple replicas in Kubernetes helps distribute the load and handle more requests.
 > Service Discovery --> if we have 3 Replica sets, if one RS down then another RS pod will be created but ip will be changing, so users not be aware of it ip change. so here svc looks for labels & selectors, so service looks for labels not ip address.
 > Load balancing  --> Expose to External world
     > Cluster ip --> if svc as cluster --> then it will access those who have access to cluster only.
     > Node Port  --> if svc as node port, then it willl access those who have access to Node Port only.
     > Load balancer --> if svc as LB, then it will access to whole world.
