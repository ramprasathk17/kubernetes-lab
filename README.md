# kubernetes-lab
What is a Pod?
A Pod is the smallest deployable unit in Kubernetes. 
It represents a single instance of a running process in a cluster.

A Pod can contain:
One container (most common case)
Multiple tightly coupled containers (sidecar pattern)
All containers inside a Pod:
Share the same network namespace (same IP address)
Share storage volumes
Are scheduled together on the same node
In production, we rarely deploy standalone Pods directly. Instead, we use higher-level controllers like Deployments to manage Pods.

What are resource requests?
Resource requests define the minimum amount of CPU and memory a container requires.
  
What happens if the limit is exceeded?
Resource limits define the maximum amount of CPU and memory a container can use.
