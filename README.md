# MongoDB-atlas-kubernetes-connector
1. Install Kubectl.  The Kubernetes command-line tool, kubectl, allows you to run commands against Kubernetes clusters. You can use kubectl to deploy applications, inspect and manage cluster resources, and view logs.
 
   
```brew install kubectl


2. Install docker desktop as hypervisor on https://docs.docker.com/desktop/install/mac-install/ Minikube uses a container runtime like Docker to run and manage containers on the worker node. Docker is one of the most popular container runtimes, but you can also configure Minikube to use other runtimes like containerd.
On macOS, Minikube requires a hypervisor to create and manage the virtual machine where the Kubernetes cluster runs. HyperKit is a lightweight hypervisor optimized for Apple Silicon (ARM-based) Macs and is used as the default hypervisor for Docker Desktop.

3. Install MiniKube. Minikube is a tool that helps you run a single-node Kubernetes cluster on your local machine. It sets up a lightweight, isolated environment where you can experiment with Kubernetes without the need for a full-scale cluster.
```brew install minicube

```
 +----------------+       +----------------+       +-----------------------+
 |                |       |                |       |                       |
 |   kubectl      +------>+    Minikube    +------>+  Local Kubernetes     |
 |                |       |                |       |    Cluster            |
 +-------^--------+       +------+---------+       +-----------------------+
         |                         |
         |                         |     +------------------------+
         |                         +---->+                        |
         |                               |  Docker (Container    |
         |                               |  Runtime)             |
         |                               +------------------------+
         |
         |       +---------------------------------+
         +------>+                                 |
                 |    Hypervisor (e.g., HyperKit)  |
                 +---------------------------------+

```




