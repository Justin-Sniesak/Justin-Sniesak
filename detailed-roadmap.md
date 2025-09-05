```
├── Go
│   ├── Cleanup old Kubernetes repo | (3) DTV modules | purple pod manifest 1
│   ├── Create pipeline repo | (3) DTV modules | purple pod manifest 2
│   ├── Attach GCP project to orginization and enable VM scanning | (3) DTV modules | purple pod manifest 3
│   ├── Create pod/PV/PVC manifest for ARGO & MongoDB |  (3) DTV modules | purple pod manifest 4
│   ├── Provision buckets/configure IAM using TF and configure IAM settings | (3) DTV modules | purple pod manifest 5
│   ├── Create K8 secrets for MongoDB users and Argo SA | (3) DTV modules | purple pod manifest 6
│   ├── compute.tf - VSC install; change all IP to ephimeral; inject RSA keys; add new VMs to SSH script | (3) DTV modules | purple pod manifest 7
│   ├── Write script for DB/Table/Users (Mongo & Argo)| (3) DTV modules | purple pod manifest 8
│   ├── Create and upload architectural diagram | (3) DTV modules | purple pod manifest 9
│   ├── Update all manifests to Deployment/ReplicaSet with rolling updates; group pods per use case | (3) DTV modules | purple pod manifest 9
│   ├── vpc.tf - Provision VPC with ephimeral IP assignment using TF and configure VPC Firewall rules | (3) OCF modules 


 
│   ├── Build Argo pipeline using Mongo & Argo manifests and K8 secrets 
Test pipeline, confirm working and correct/document any issues |
│   ├── Configure Prometheus pod; self monitoring; configure dashboard; expose externally | Configure argo, write additional manifest and merge to repo, confirm pipeline is merging and pulling new code | (3) OCF modules | purple pod manifest 6
(3) OCF modules | purple pod manifest 7
│   ├── Push all updated deployment manifests to repo and test, confirm updates and restarts are being applied as intended | (3) OCF modules | purple pod manifest 8
│   ├── Configure argo and pipeline to ImagePull: Latest with auto restart of pods | (3) OCF modules | purple pod manifest 9
│   ├── Write imperative run book for every step in GCP deployment, pipeline/argo & K8 cluster - attach to repo | (3) OCF modules | purple pod manifest 9
│   ├── Arays, slices and maps
│   ├── Using Functions
│   ├── Pointers
│   ├── Struct, Methods and Interfaces
│   └── Conclusion
├── GKE
│   ├── Add tags to buckets storage.tf
│   ├── Update deployment manifest, install Prometheus agent on all containers via daemonset, validate data is being ingested properly - validate 
│   ├── Cleanup Docker repo
│   ├── Go script to provide VM name & IP upon Terraform creation in TXT file- Automate
│   ├── Cleanup Python repo
│   └── Configure service account IAM tagging in GCP 
├── Helm
│   ├── master.tf - update to install Prometheus agent on all Ubuntu guests, validate data is being ingested properly - validate
│   ├── Update container security in all pods via Deployment manifest 
│   ├── Update compute.tf to inject RSA keys into VMs 
│   ├── Update auth IAM tag for compute SA to pull available OS images from GCP
│   ├── Kubernetes Cluster: Install ProxMox Hypervisor
│   └── Add HPA to Deployment manifest 
├── Rust
│   ├── Create Grafana dashboard and cutover from Prometheus - ensure all data is being ingested properly 
│   ├── Kubernetes Cluster: Install ProxMox Hypervisor
│   ├── Add VPA to Deployment manifest 
│   ├── Remap cluster PVs to GCP buckets 
│   ├── Update pod startup commands in Deployment manifest 
│   └── Containerize and add Ollama, nodeJS, mcp/jetbrains to Deployment manifest; add to monitoring (Prometheus/Grafana); connect to VMs (Unidirectional 1:1) 
├── CKA
│   ├── Kubernetes Cluster: Provision and configure (4) Ubuntu Linux guests along with VSC, map to containers - Ollama, nodeJS, Go, mcp/jetbrains 
│   ├── GCP Infrastructure: Provision VM, install Terraform, scp over .tf files from Bastion Host
│   ├── Join Kubernetes SIG Networking
│   └── GCP Infrastructure: Using Terraform, provision and configure (4) VMs with each having Nginx, VSC and Chrome installed
├── Go (Intermediate)
│   ├── Kubernetes Cluster: Provision and configure master and (3) worker node Kubernetes cluster on guests
│   ├── Kubernetes Cluster: Create, deploy and automate Go scripts
│   └── GCP Infrastructure: Configure DNS management for all VMs
├── GCP Cloud Digital Leader
│   ├── Kubernetes Cluster: Provision, test and configure Rook-ceph cluster
│   ├── Kubernetes Cluster: Provision test and configure containers for the following: Nginx, Prometheus, Python, Loki, Chromium/Ubuntu desktop, Anthropic MCP (Ollama), Redis, GitHub actions, MongoDB 
│   └── GCP Infrastructure: Connect, test and configure Kubernetes cluster to GCP storage bucket
├── PCA
│   ├── Kubernetes Cluster: Build out and configure Grafana dashboard for each cluster
│   ├── GCP Infrastructure: Configure VPC firewall rules
│   └── GCP Infrastructure: Provision and configure GKE cluster across all VMs (5 Node cluster - (1) master, (4) workers)
├── Go (Advanced)
│   ├── Kubernetes Cluster: Configure, test and deploy external reachability
│   ├── GCP Infrastructure: Configure, test and deploy external reachability
│   └── TBD
├── CGOA
│   └── TBD
├── GCP ACE
│   └── TBD
├── CBA
│   └── TBD
├── CKS
│   └── TBD
├── ICA
│   └── TBD
├── CCA
│   └── TBD
