**Kubernetes** is an open source container orchestration platform that automates many of the manual processes involved in deploying, managing, and scaling containerized applications.

**Minikube** is a tool that sets up a Kubernetes environment on a local PC or laptop. It’s technically a Kubernetes distribution, but because it addresses a different type of use case than most other distributions (like Rancher, OpenShift, and EKS), it’s more common to hear folks refer to it as a tool rather than a distribution.
Minikube supports all of the major operating systems – Windows, Linux, and macOS. (It doesn’t run on mobile devices, alas.)
**K3d** is a lightweight wrapper to run k3s (Rancher Lab’s minimal Kubernetes distribution) in docker.
k3d makes it very easy to create single- and multi-node k3s clusters in docker, e.g. for local development on Kubernetes.
**Kind** is a tool for running local Kubernetes clusters using Docker container “nodes”.
kind was primarily designed for testing Kubernetes itself, but may be used for local development or CI.

|             **key**              |          **minikube**          |       **kind**       |                **k3d**                |
|:--------------------------------:|:------------------------------:|:--------------------:|:-------------------------------------:|
|               _OS_               |       Linux,MacOS,Windows      |  Linux,MacOS,Windows |          Linux,MacOS,Windows          |
|            _runtime_             |               VM               |       container      |                 native                |
|    _supported architectures_     |              AMD64             |         AMD64        |          AMD64, ARMv7, ARM64          |
| _supported container runtimes_   | Docker,CRI-O,containerd,gvisor |        Docker        |           Docker, containerd          |
|          _startup time_          |             29,448s            |        19,691s       |                 15,576s               |
|      _memory requirements_       |               2GB              | 8GB (Windows, MacOS) |                  512 MB               |
|         _requires root?_         |                no              |           no         |     yes (rootless is experimental)    |
|     _multi-cluster support_      |               yes              |          yes         | no (can be achieved using containers) |
|       _multi-node support_       |                no              |          yes         |                  yes                  |
|               _GUI_              |               yes              |           no         |                  yes                  | 
|   _possibility of using Podman_  |      yes (experimental)        |          yes         |                  yes                  |
|        _stars on GitHub_         |              25.8k             |         11.1k        |                  4.1k                 |
|      _mounting local code_       |               yes              |           no         |                  yes                  |
