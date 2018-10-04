_This is a list of resources for all thingz stateful apps and tooling in and for Kubernetes. I did an initial dump of my bookmarks here but would really appreciate it if you heavily [PR it](https://github.com/mhausenblas/stateful-kubernetes/pulls), or if you don't feel comfortable doing this, at least raise an [issue](https://github.com/mhausenblas/stateful-kubernetes/issues) for what's missing. If you send in suggestions or update the resources directly, please also add yourself to the [list of contributors](https://github.com/mhausenblas/stateful-kubernetes/blob/master/CONTRIBUTORS) using a website, an mail address or a Twitter handle to sign off._

---

Note: when you read _in-tree_ it means it's part of the Kubernetes source code, otherwise we call it _3rd-party_, that is, using some kind of [Kubernetes extensibility](https://speakerdeck.com/mhausenblas/bending-kubernetes-to-your-needs) mechanism.

## Storage

Official Kubernetes docs and specifications.

### In-Tree Storage

- [Volumes](https://kubernetes.io/docs/concepts/storage/volumes/)
- [Configuring a pod to use a volume](https://kubernetes.io/docs/tasks/configure-pod-container/configure-volume-storage/)
- [Persistent Volumes](https://kubernetes.io/docs/concepts/storage/persistent-volumes/) (PVs)
- [Configuring a pod to use a PV](https://kubernetes.io/docs/tasks/configure-pod-container/configure-persistent-volume-storage/)
- [Dynamically provisioning PVs](https://kubernetes.io/docs/concepts/storage/dynamic-provisioning/) via [storage classes](https://kubernetes.io/docs/concepts/storage/storage-classes/)

### 3rd-Party Storage

- [Container Storage Interface (CSI)](https://github.com/container-storage-interface/spec)

### Blog Posts and Articles

- 08/2018: [Dynamically Expand Volume with CSI and Kubernetes](https://kubernetes.io/blog/2018/08/02/dynamically-expand-volume-with-csi-and-kubernetes/)
- 06/2018: [How to write a Container Storage Interface (CSI) plugin](https://arslan.io/2018/06/21/how-to-write-a-container-storage-interface-csi-plugin/)
- 04/2018: [Container Storage Interface (CSI) for Kubernetes Goes Beta](https://kubernetes.io/blog/2018/04/10/container-storage-interface-beta/)
- 01/2018: [Introducing Container Storage Interface (CSI) Alpha for Kubernetes](https://kubernetes.io/blog/2018/01/introducing-container-storage-interface/)
- 12/2017: [Troubleshooting: Unable to mount volumes for pod because “volume is already exclusively attached to one node and can’t be attached to another”](https://portworx.com/warning-failedattachvolume-warning-failedmount-kubernetes-aws-ebs/)
- 12/2017: [A Basic Guide to Kubernetes Storage](https://portworx.com/basic-guide-kubernetes-storage/)
- 05/2017: [Kubernetes: State and Storage](https://blog.openshift.com/kubernetes-state-storage/)
- 10/2016: [Dynamic Provisioning and Storage Classes in Kubernetes](https://kubernetes.io/blog/2016/10/dynamic-provisioning-and-storage-in-kubernetes/)

### Videos and Slide Decks

- [Stateful Applications in Kubernetes: Ready for Production!](https://speakerdeck.com/ntolia/stateful-applications-in-kubernetes-ready-for-production)
- [Approaches for duplicating Kubernetes storage with Gluster](https://www.youtube.com/watch?v=NaYTP9OKwdk)
- [Persistent Storage with Kubernetes in Production - Which Solution and Why?](https://www.youtube.com/watch?v=hqE5c5pyfrk)
- [Kubernetes Storage Lingo 101 - Saad Ali, Google (Beginner Skill Level)](https://www.youtube.com/watch?v=uSxlgK1bCuA)
- [Tutorial: Introduction to Stateful Applications on Kubernetes](https://www.youtube.com/watch?v=B-791PMq4cU)
- [Container Engine: Storage Classes & Dynamic Provisioning in Kubernetes](https://www.youtube.com/watch?v=qktFhjJmFhg)
- [Using Kubernetes Local Storage for Scale-Out Storage Services](https://www.youtube.com/watch?v=eqkgiPppZN8)
- [Intro to Container Storage Interface (CSI)](https://www.youtube.com/watch?v=_EFJeIQzbmo)


### Projects and Products

- Public cloud
  - Amazon [EKS Storage Classes](https://docs.aws.amazon.com/eks/latest/userguide/storage-classes.html)
  - Google [GKE Storage](https://cloud.google.com/kubernetes-engine/docs/concepts/storage-overview)
  - Microsoft Azure [AKS Persistent Volumes](https://docs.microsoft.com/en-us/azure/aks/azure-disks-dynamic-pv)
- On-premises and cross-cloud
  - [CephRBD](https://access.redhat.com/products/red-hat-ceph-storage)
  - [GlusterFS](https://github.com/gluster/gluster-kubernetes)
  - [MapR Data Fabric for Kubernetes](https://mapr.com/solutions/data-fabric/kubernetes/)
  - [OpenEBS](http://github.com/openebs/openebs/)
  - OpenStack [Cinder](http://wiki.openstack.org/cinder)
  - [Portworx](https://docs.portworx.com/scheduler/kubernetes/)
  - [Quobyte](https://github.com/quobyte/kubernetes)
  - [Rook](http://rook.io/)
  - [StorageOS](http://storageos.com)
  - [Stork](https://github.com/libopenstorage/stork)
  - [NetApp Trident](https://github.com/NetApp/trident)
- Chaos Engineering frameworks
  - [Litmus](https://github.com/openebs/litmus)

## Datastores and Operators

### Official Kubernetes Docs and Specifications

- [StatefulSets](https://kubernetes.io/docs/concepts/workloads/controllers/statefulset/)
- [Run a Single-Instance Stateful Application](https://kubernetes.io/docs/tasks/run-application/run-single-instance-stateful-application/)
- [Controller](https://kubernetes.io/docs/reference/glossary/?fundamental=true#term-controller)
- [Custom Resources](https://kubernetes.io/docs/concepts/extend-kubernetes/api-extension/custom-resources/)
- [Extend the Kubernetes API with custom resources](https://kubernetes.io/docs/tasks/access-kubernetes-api/custom-resources/custom-resource-definitions/)

### Blog posts and Articles

- 09/2018: [How to Install Redis Enterprise Clusters Using Operators on OpenShift](https://redislabs.com/blog/install-redis-enterprise-clusters-using-operators-openshift/)
- 08/2018: [Getting Started with Apache Kafka and Kubernetes](https://www.confluent.io/blog/getting-started-apache-kafka-kubernetes/)
- 08/2018: [Getting started with MongoDB Enterprise Operator for Kubernetes](https://hackernoon.com/getting-started-with-mongodb-enterprise-operator-for-kubernetes-bb5d5205fe02)
- 06/2018: [Kubernetes StatefulSet In Action](https://blog.openshift.com/kubernetes-statefulset-in-action/)
- 05/2018: [A complete guide to Kubernetes Operator SDK](https://banzaicloud.com/blog/operator-sdk/)
- 05/2018: [Introducing the Operator Framework: Building Apps on Kubernetes](https://coreos.com/blog/introducing-operator-framework)
-05/2018: [PostgreSQL Kubernetes: How to run HA Postgres on Kubernetes](https://portworx.com/ha-postgresql-kubernetes/)
- 04/2018: [Comparing Kubernetes Operator Pattern with alternatives](https://medium.com/@cloudark/why-to-write-kubernetes-operators-9b1e32a24814)
- 04/2018: [Kubernetes Persistent Volumes with Deployment and StatefulSet](https://akomljen.com/kubernetes-persistent-volumes-with-deployment-and-statefulset/)
- 04/2018: [How to run HA MongoDB on Kubernetes](https://portworx.com/ha-mongodb-kubernetes/)
- 03/2018: [Why Kubernetes Operators are a game changer](https://blog.couchbase.com/kubernetes-operators-game-changer/)
- 03/2018: [Introducing the Oracle MySQL Operator for Kubernetes](https://blogs.oracle.com/developers/introducing-the-oracle-mysql-operator-for-kubernetes)
- 12/2017: [Kubernetes Elasticsearch Operator](https://akomljen.com/kubernetes-elasticsearch-operator/)
- 08/2017: [Kubernetes WordPress: How to run HA WordPress on Kubernetes](https://portworx.com/kubernetes-wordpress-ha/)
- 08/2017: [MySQL Kubernetes: deploying and running MySQL on Kubernetes using statefulsets and kops](https://portworx.com/mysql-kubernetes/)
- 03/2017: [PostgreSQL Operator for Kubernetes](https://info.crunchydata.com/blog/postgres-operator-for-kubernetes)
- 03/2017: [A new “Kafka” novel : the OpenShift & Kubernetes deployment](https://paolopatierno.wordpress.com/2017/03/25/a-new-kafka-novel-the-openshift-kubernetes-deployment/)
- 03/2017: [Rook Operator: First class storage for Kubernetes](https://blog.rook.io/rook-operator-first-class-storage-for-kubernetes-2d0288831175)
- 02/2017: [Deploying PostgreSQL Clusters using StatefulSets](https://kubernetes.io/blog/2017/02/postgresql-clusters-kubernetes-statefulsets/)
- 02/2017: [Two days of pain or how I deployed GlusterFS to Kubernetes](https://blog.lwolf.org/post/how-i-deployed-glusterfs-cluster-to-kubernetes/)
- 01/2017: [Running MongoDB on Kubernetes with StatefulSets](https://kubernetes.io/blog/2017/01/running-mongodb-on-kubernetes-with-statefulsets/)
- 12/2016: Hacker News thread on [StatefulSet: Run and Scale Stateful Applications Easily in Kubernetes](https://news.ycombinator.com/item?id=13225183)
- 11/2016: [Original CoreOS Operators launch explainer](https://coreos.com/blog/introducing-operators.html)

### Videos and Slide Decks

- [High Availability for Stateful GKE Workloads](https://www.youtube.com/watch?v=rRZtZX0PDFc)
- [Why You Care About Kubernetes Operators](https://www.youtube.com/watch?v=6Csf0g9BTr4)
- [A Kubernetes Operator for PostgreSQL - Architecture and Design](https://www.youtube.com/watch?v=LwIOoU96iQw)
- [Elasticsearch on Kubernetes](https://speakerdeck.com/joerx/elasticsearch-on-kubernetes)

### Projects and Products

- Datastores
  - [Vitess](https://vitess.io/), a database clustering system for horizontal scaling MySQL
  - [Kafka](https://www.confluent.io/resources/recommendations-for-deploying-apache-kafka-on-kubernetes)
  - [MariaDB Galera](https://github.com/adfinis-sygroup/mariadb-galera-chart) Helm chart
- Operators
  - [KubeDB - Run production-grade databases easily on Kubernetes](https://kubedb.com/)
  - [Operator SDK](https://github.com/operator-framework/operator-sdk)
  - [Awesome Operators in the Wild](https://github.com/operator-framework/awesome-operators)
  - [Kanister - An Operator Focused on App-Level Data Management](https://github.com/kanisterio/kanister)
  - [Node Disk Manager for Kubernetes](https://github.com/openebs/node-disk-manager)
  - [Introducing the Confluent Operator: Apache Kafka on Kubernetes Made Simple](https://www.confluent.io/blog/introducing-the-confluent-operator-apache-kafka-on-kubernetes/)
  - [KubeDirector](https://github.com/bluek8s/kubedirector)

## Backup and restore

### Official Kubernetes Docs and Specifications

- None yet

### Blog Posts and Articles

- 09/2018: [How to backup and restore MySQL on Red Hat OpenShift](https://portworx.com/backup-restore-mysql-red-hat-openshift/)

### Videos and Slide Decks

- None yet

### Projects and Products

#### Cross-platform

- [Kasten's K10 Platform](https://kasten.io/product/)
- [Heptio Ark](https://github.com/heptio/ark)
- [ReShifter](http://reshifter.info/)
- [Stash by AppsCode - Backup your Kubernetes Volumes](https://github.com/appscode/stash)

#### Database-specific

- [KubeDB - Run production-grade databases easily on Kubernetes](https://github.com/kubedb)
- [Kanister - Cross-data service backup and restore](https://github.com/kanisterio/kanister)

#### Storage-system specific

- [Portworx PX-Enterprise](https://docs.portworx.com/cloud/backups.html#multi-cloud-backup-and-recovery-of-px-volumes)
