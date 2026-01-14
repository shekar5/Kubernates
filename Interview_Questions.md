1Q) what is difference of Docker and kubernates ?
A ) Docker is a container platoform, kubernates is a container orchestration platform. Cluster , Auto Healing , Auto scaling and enterprise level like load balancer.support.

2)what are the main components of Kubernetes architecture ?
Control plane - (master)
Api server --> which handles API, talking to end users.
scheduler --> which schedules
etcd --> object store
controller manager --> Replication set, controls to have same 
cloud control Manager (CCM) --> to implement on cloud provides, they will manage to have those resources.

Data Plane - (Worker Node )
Kubelet --> managing pods like healthy on nodes
kubeproxy --> networking --> updating ip-adress, svc like kube-proxy updates.
container runtime --> for a container to run like crio. D etc..

3) what are the difference b/n docker swarm and Kubernetes??
Kubernates is better suited for large org as it offers more scalability, networking capabilities and huge third party ecosystem support.

4.what is dff b/n docker container and a kubernates pod ?
A ) A pod in kubernates is a runtime specification of a container in docker. A pod provides more declaratibe way of defining using yaml and you can run more than one container in a pod.

5.what is namespace in kubernates ?
A)   In kubernates namespaces is a logical isolation of resources, network policies , rbac and everything. For example, there are 2 projects using same k8 cluster. one project can use ns1 and other project can use ns2 without andy overlap and authentication.
