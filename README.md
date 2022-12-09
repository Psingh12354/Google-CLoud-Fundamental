<h1 align='center'> Google-CLoud-Fundamental</h1>

### Notes
- Anything which we create here is considered as resources
- Resources belong to projects
- Project may be organized into folders.
- Folder belong to an organization and it's provide logical grouping of projects.
- Google cloud Interaciton
  - Web console
  - Cloud Shell Coud SDK
  - Mobile App
  - Rest API

### Footprint of google cloud
- 20 Regions(Collection of multiple data center have atleast 2 zones)
- 61 Zones(It is the location like delhi mumbai they are considered to be zones)
- 134 Network Edge location
- Available in 200+ Countries and terriotries

### Compute
- Compute Engine
- APP Engine
- Kubernetes Engine
- Container Registry
- Cloud Functions

### Storage and Databases
- Cloud Storage
- Cloud Bigtable
- Cloud Datastore
- Cloud Sql
- Cloud Spanner
- Persistent Disk

### Networking
- Cloud Virtual Network
- Cloud Load Balancing
- Cloud CDN
- Cloud Internconnect
- Cloud DNS

### Security & Identity
- Cloud IAM(Identity & access managemnet)
- Cloud Resource Manager
- Cloud Security Scanner
- Cloud Platform Security

### AI  & Machine learning
- Cloud Machine Learning 
- Vision API
- Speech API
- Natural Language API
- Translation API
- Jobs API

### DevOps(Development + Operations) Tools
- Cloud SDK
- Deployement Manager
- Cloud Source Repositories
- Cloud Tools for Android Studio
- Cloud Tools for IntelliJ
- PowerShell Cloud Tools
- Visual Studio Cloud Tools
- Plug-in for Eclipse 
- Cloud Test Lab

### Cloud Shell

- To get all availble regions ```gcloud compute regions list```
- To get instance list ```gcloud compute instance list```
- Can inject some data in instance by using ```gcloud compute ssh instance-1 --zone asia-south1-a```
- ssh stands for secure shell enables computer to communication here it help to communication multiple VMs.
- Update ```sudo apt-get update```

### Google App Engine

- One of the first compute services from Google(PaaS)

### Google Compute Engine

- Enable Linux and Windows Vms to run on google global infrasturcture
- VMs have different configuration
- Persistence is available through statdard and SSD disk.

### Google Kubernetes Engine

- Managed Environment for deploying container
- Kubernetes has a control plane and worker node
- Auto Scaling, Automatic upgrades and node auto-repair are features of GKE

### Google Cloud Functions

- Cloud functions is a serverless execution environment for building and connecting cloud services.
- Support JavaScript, Python3, and Go
- GCP events Fire a cloud functions through trigger
- Trigger connects the event to funciton

### Why do we need GCP Storage?

- To make it persistent and durable
- Storage services are classified in three types-: 
  - Object Storage
  - Block Sotrage
  - File system
- Unified storage for variety of application
- 99.99% durability.
- Data can be stored in one region or multiple region
- Storage class
  - High frequency Access(standard most common storage class used by developer optimized for reduce latency.)
  - Low Frequency Access(Nearline meant for data access less frequently)
  - Lowest frequency access(Coldline data access in a year)
  
### Persistent Disks

- Disk are Independent of Compute Engine VMs.
- max 64TB.
- Work like pubsub
- SSD and HDD
- PD available in three storage types-:
  - Zonal
  - Regional
  - Local
  
  ### Google filestore
  
  - Filestore instances are fully managed NFS file servers on Google Cloud for use with applications running on Compute Engine virtual machines (VMs) instances or Google Kubernetes Engine clusters.
  - **Network File System (NFS)** is a distributed file system protocol originally developed by Sun Microsystems (Sun) in 1984, allowing a user on a client computer to access files over a computer network much like local storage is accessed.

### Google bucket

- You store objects in containers called buckets. All buckets are associated with a project, and you can group your projects under an organization. Each project, bucket, and object in Google Cloud is a resource in Google Cloud, as are things such as Compute Engine instances.

### GCP Network Service Tiers

- Traffic optimization
- Two service tiers-:
  - Premimum Tier(default one here traffic via google premium backbone)
  - Standard Tier(Connectivity based on ISP networks)
 
### Load balancer 

- help to distributes traffic in multple GCE Vms in a region or multiple region
- Two types of load balancer-:  
  - HTTP(s) load balancer (Global load balancing)
  - Network Load balancer(Regional TCP and UDP traffic)

### Virtual Private Cloud(VPC)

- Provide private networking VMs
- Subnets are part of large network it means sub networking
- Each VPC is logivally isolated
- Protected by Firewall
- VPC network can be connected to each other via VPC Peering.

### IAM

- Who(Identify) has what access(Role) for which resource.
- least privilege
- Primitive roles-:
  - Owner(100%)
  - Editor(who can view and edit)
  - Viewer(oly view)
- Predefined roles
  - roles/pubsub.publisher
  - roles/compute.admin
  - roles/storage.objectAdmin 

### Google cloud sql

- No need of VMs managed rdbms
- Three types of RDBMS
  - MySql
  - PostgreSql
  - Microsoft Sql server
- Google cloud dataproc(use to work with apache spark and hive like tool)
- Google cloud datalab(It is use for analysis and visualization support python, sql, javascript)

### BigQuery

- It is use to deal with analysis job
- Datawarehouse purpose
- Query large dataset in ANSI SQL.
