```
├── Go 
│   ├── Create GitHub repo
│   ├── Cleanup old Kubernetes repo
│   ├── Attach GCP project to orginization and enable VM scanning (GCP)
│   ├── Provision buckets using TF and configure IAM settings (TF)
│   ├── Data Types and Variables
│   ├── compute.tf - VSC install; change all IP to ephimeral; inject RSA keys; add new VMs to SSH script (TF)
│   ├── Create and upload architectural diagram (Enterprise)
│   ├── Provision VPC with ephimeral IP assignment using TF and configure VPC Firewall rules(TF)
│   ├── Operators and Control Flow
│   ├── Configure Prometheus pod; self monitoring; configure dashboard; expose externally (Prom)
│   ├── Convert master PV pod manifest to Deployment include ReplicaSet in cluster (K8)
│   ├── Add tags to buckets storage.tf (TF)
│   ├── Arays, slices and maps
│   ├── Update deployment manifest, install Prometheus agent on all containers via daemonset, validate data is being ingested properly - validate (Prom)
│   ├── Cleanup Docker repo
│   ├── Go script to provide VM name & IP upon Terraform creation in TXT file- Automate (TF)
│   ├── Using Functions
│   ├── Cleanup Python repo
│   ├── Configure service account IAM tagging in GCP (GCP)
│   ├── master.tf - update to install Prometheus agent on all Ubuntu guests, validate data is being ingested properly - validate (TF)
│   ├── Pointers
│   ├── Update container security in all pods via Deployment manifest (K8)
│   ├── Update compute.tf to inject RSA keys into VMs (TF)
│   ├── Update auth IAM tag for compute SA to pull available OS images from GCP (GCP)
│   ├── Struct, Methods and Interfaces
│   ├── Kubernetes Cluster: Install ProxMox Hypervisor
│   ├── Add HPA to Deployment manifest (K8)
│   ├── Create Grafana dashboard and cutover from Prometheus - ensure all data is being ingested properly (Grafana)
│   └── Conclusion
├── GKE
│   ├── Kubernetes Cluster: Install ProxMox Hypervisor
│   ├── Add VPA to Deployment manifest (K8)
│   └── Remap cluster PVs to GCP buckets (K8)
├── Helm
│   ├── Update pod startup commands in Deployment manifest (K8)
│   ├── Containerize and add Ollama, nodeJS, mcp/jetbrains to Deployment manifest; add to monitoring (Prometheus/Grafana); connect to VMs (Unidirectional 1:1) (K8)
│   └── Kubernetes Cluster: Provision and configure (4) Ubuntu Linux guests along with VSC, map to containers - Ollama, nodeJS, Go, mcp/jetbrains (K8)
├── CKA
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
