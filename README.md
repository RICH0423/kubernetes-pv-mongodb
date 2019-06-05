## Deploy MongoDB on Kubernetes using PersistentVolume

This project is to demo how to deploy MongoDB on Kubernetes using PersistentVolume.
The purpose of using PersistentVolume(PV) &  ersistentVolumeClaim (PVC) is to decouple the pod from the storage.

- A PersistentVolume (PV) is a piece of storage in the cluster that has been provisioned by an administrator.
  - PersistentVolumes are cluster-level resources.
  - PersistentVolumes has its own life cycle

- A PersistentVolumeClaim (PVC) is a request for storage by a user. 

## Steps to create your PV/PVC
1. Cluster administrator sets up the storage and then registers it in Kubernetes by creating a PersistentVolume resource.

2. When a user needs to use persistent storage, they first create a PersistentVolumeClaim manifest, specifying the minimum size and the access mode they require then submits it. 

3. Kubernetes finds the appropriate PersistentVolume and binds the volume to the claim.
