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

6) what is the role of kube-proxy ?
A) kube-proxy works by maintaining a set of network ruleson each node in the cluster, which are updated dynamically as services are added or removed. when a client sends a request to a service, the request is intercepted by kube-proxyon the node where its received.kube-proxy then looks  up the destination endpoint for the service and routes the request accordingly.

kube-proxy is an essential component of a kubernates cluster , as it ensures that services can communicate with each other.

7)what are the diff types of services within kubernates ??
A) > cluster-ip Mode
   > Node-port Mode
   > Load balancer Mode

8)what is diff b/n nodeport and Load balancer type service ?
A)when as service is created a Nodeport tyoe, The kube-proxy updates the IP Tables with Node Ip Address and port that is choosen in the service configuration to access the pods.

Where as if you create a service as type LoadBalancer, the cloud control manager creates a external load balance ip using the underlying cloud provider logic in the CCm. users can access services using the external ip .

9)What is the role of kubelet ??
A) Kubelet manages the containers that are scheduled to run on that node.It ensures that node. It ensures that the containers are running and healthy and that the resources they need are available.

Kubelet communicates with the kubernates API server to get information about containers that should be running on the node and then starts and stops the containers as needed to maintain the desired state. It also monitors the containers to ensure that they are running correctly and restarts them if necessary.

10)Day to Day activities on kubernates ??
A) We have 3 master Nodes and 10 worker Nodes, we will maintain version upgrades, avoid vulnerabilities and will help Apps Team to troublehoot if they any issue and also we get tickets / Jira Tickets if any issues, based on we will schedule call and troubleshoot accordingly.
