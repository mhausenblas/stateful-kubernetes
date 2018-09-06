_This is a list of resources for all thingz stateful apps and tooling in and for Kubernetes. I did an initial dump of my bookmarks here but would really appreciate it if you heavily [PR it](https://github.com/mhausenblas/stateful-kubernetes/pulls), or if you don't feel comfortable doing this, at least raise an [issue](https://github.com/mhausenblas/stateful-kubernetes/issues) for what's missing. If you send in suggestions or update the resources directly, please also add yourself to the [list of contributors](CONTRIBUTORS) using a website, an mail address or a Twitter handle to sign off._

---

Note: when you read _in-tree_ it means it's part of the Kubernetes source code, otherwise we call it _3rd-party_, that is, using some kind of [Kubernetes extensibility](https://speakerdeck.com/mhausenblas/bending-kubernetes-to-your-needs) mechanism.

## Storage

Official Kubernetes docs and specifications.

In-tree storage:

- [Volumes](https://kubernetes.io/docs/concepts/storage/volumes/)
- [Configuring a pod to use a volume](https://kubernetes.io/docs/tasks/configure-pod-container/configure-volume-storage/)
- [Persistent Volumes](https://kubernetes.io/docs/concepts/storage/persistent-volumes/) (PVs)
- [Configuring a pod to use a PV](https://kubernetes.io/docs/tasks/configure-pod-container/configure-persistent-volume-storage/)
- [Dynamically provisioning PVs](https://kubernetes.io/docs/concepts/storage/dynamic-provisioning/) via [storage classes](https://kubernetes.io/docs/concepts/storage/storage-classes/)

3rd-party storage:

- [Container Storage Interface (CSI)](https://github.com/container-storage-interface/spec)

Blog posts and articles:

- 08/2018: [Dynamically Expand Volume with CSI and Kubernetes](https://kubernetes.io/blog/2018/08/02/dynamically-expand-volume-with-csi-and-kubernetes/)
- 04/2018: [Container Storage Interface (CSI) for Kubernetes Goes Beta](https://kubernetes.io/blog/2018/04/10/container-storage-interface-beta/)
- 01/2018: [Introducing Container Storage Interface (CSI) Alpha for Kubernetes](https://kubernetes.io/blog/2018/01/introducing-container-storage-interface/)
- 12/2017 [A Basic Guide to Kubernetes Storage](https://dzone.com/articles/a-basic-guide-to-kubernetes-storage)
- 05/2017: [Kubernetes: State and Storage](https://blog.openshift.com/kubernetes-state-storage/)
- 10/2016: [Dynamic Provisioning and Storage Classes in Kubernetes](https://kubernetes.io/blog/2016/10/dynamic-provisioning-and-storage-in-kubernetes/)

Videos and slide decks:

- [Persistent Storage with Kubernetes in Production - Which Solution and Why?](https://www.youtube.com/watch?v=hqE5c5pyfrk)

Projects and products:

- Public cloud
  - Amazon [EKS Storage Classes](https://docs.aws.amazon.com/eks/latest/userguide/storage-classes.html)
  - Google [GKE Storage](https://cloud.google.com/kubernetes-engine/docs/concepts/storage-overview)
  - Microsoft Azure [AKS Persistent Volumes](https://docs.microsoft.com/en-us/azure/aks/azure-disks-dynamic-pv)
- On-premises and cross-cloud
  - [CephRBD](https://access.redhat.com/products/red-hat-ceph-storage)
  - [GlusterFS](https://github.com/gluster/gluster-kubernetes)
  - [OpenEBS](http://github.com/openebs/openebs/)
  - OpenStack [Cinder](http://wiki.openstack.org/cinder)
  - [Portworx](https://docs.portworx.com/scheduler/kubernetes/)
  - [Quobyte](https://github.com/quobyte/kubernetes)
  - [Rook](http://rook.io/)
  - [StorageOS](http://storageos.com)
  - [Stork](https://github.com/libopenstorage/stork)

## Operators

Official Kubernetes docs and specifications:

Blog posts and articles:

Videos and slide decks:

Projects and products:

## Datastores

Official Kubernetes docs and specifications:

Blog posts and articles:

Videos and slide decks:

Projects and products:

## Backup and restore

Official Kubernetes docs and specifications:

Blog posts and articles:

Videos and slide decks:

Projects and products:
