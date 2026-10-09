## Local Kubernetes Environment

This project uses Rancher Desktop's local k3s cluster instead of the course
Vagrant/VirtualBox VM. My company windows pc does not provide administrator
permissions, and the Vagrant VM could not start because VirtualBox's
`VBoxHeadless.exe` process crashed with Windows error `0xc0000005`. Therefore Rancher Desktop was used.

Rancher Desktop provides a supported local Kubernetes environment without
requiring administrator access. Its node runs k3s, as indicated by the
Kubernetes version suffix `+k3s1`.

$ kubectl version  
Client Version: v1.36.3  
Kustomize Version: v5.8.1  
Server Version: v1.36.3+k3s1  
