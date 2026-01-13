Docker --> Docker is container platflorm
Kubernates --> Container Orchestaration platform.

Docker contains only below , but not docker swarm
> Single Host  --> if single Host(Ec2) , .but nothing can do with Docker but in kubernates, its runs with cluster.
> No Auto Healing --> Docker runs mutiple Containers like 1 to 100, if 2nd container consumes more memory..it will effect 99th container also. but no Auto Healing happens, but in kubernates, it will re-create the container and move 99th working container into another Node/
> No Auto Scaling --> in Docker, we need to manually increase resources like RAM or capacity, but in kubernates it will scale up automatically using Replica sets or HPA 
> No Enterprise Level Support  --> it wont support LB, Firelwall etc to make enterprise application but in K8s, we have support LB using ingress etc

We use Kubernetes for 
> Cluster
> Auto Healing
> Auto Scaling
> Enterprose level support
