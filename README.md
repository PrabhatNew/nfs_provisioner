## Installation
1. Clone the repository to your primary master node using the following command:
   `````sh
   sudo git clone https://github.com/PrabhatNew/nfs_provisioner.git
   

2. Navigate to the repository directory:
   ````sh 
   cd nfs_provisioner


## Customization

You have to customize the NFS server details, follow these steps to set your nfs server ip and nfs path:

1. Open the deployment YAML file.
2. Find the `NFS_SERVER` and `NFS_PATH` environment variables in the container specification section.
3. Replace the `REPLACE_WITH_NFS_SERVER_IP` with the IP address or hostname of your NFS server.
4. Replace the `REPLACE_WITH_NFS_PATH` with the path to your NFS shared directory.
5. Save the changes.

After customizing the deployment YAML file, you can apply it to your Kubernetes cluster using the `kubectl apply` command:

```bash
kubectl apply -f class.yaml
```

```bash
kubectl apply -f deployment.yaml
```

```bash
kubectl apply -f rbac.yaml
```