# About Me

Thank you for visiting my GitHub. I hope your day is going well.

My career thus far has been focused on specializing in Linux (RHEL/Ubuntu), Virtualization (VMWare & KVM), and Networking (Layers 2 & 3). I have progressively moved from :

- Helpdesk
- Enterprise Operational Server Support/Administration
- Network Engineering
- Senior System Administration
- Infrastructure Engineering

I currently reside in the Seattle metro area and absolutely love it here.

**Ideal roles:** SRE or Platform Engineer.

**Primary technological focus:** Kubernetes, Go, GCP, Prometheus, Rook, GitOps, Backstage, Istio, Cilium.

I am active on here and LinkedIn almost daily, as I am passionate about working in both GCP and with cloud native technologies. It's not work if you enjoy what you do, right?

Please note, I run all my own labs locally in my own environment. I prefer this as not only do I have to set them up myself, but when I break them, I have to fix them. 

Additionally, I am a huge proponent of organized, methodical documentation, and strive to have each and every repo I work in and build adhere to this standard.

Thank you again for visiting my GitHub, and if any of this resonates with you, or you have any questions, I would love to connect and speak further, so please do not hesitate to reach out, either here, on LinkedIn, or via email.

---

### Notes
Earlier commits were not annotated due to a focus on uploading and documenting work completed while repos were being built. Additionally, I had not yet developed consistent formatting across my various repos. 
Going forward, as of 08/20/2025, in addition to consistent documentation formatting and tree structure, all commits will be annotated with what is being uploaded.

Below is a roadmap of planned certifications, courses, and projects I am or will be working on. I try to devote 10-15 hours a week to this so ideally this will all be completed in the next 15 months.

```
├── Go 
│   ├── Getting Started - Create GitHub repo
│   ├── Cleanup old Kubernetes repo
│   ├── Data Types and Variables
│   ├── compute.tf - VSC install; change all IP to ephimeral; inject RSA keys; add new VMs to SSH script
│   ├── Operators and Control Flow
│   ├── Create and upload architectural diagram
│   ├── Arays, slices and maps
│   ├── Configure Prometheus pod; self monitoring; configure dashboard; expose externally 
│   ├── Using Functions
│   ├── Convert master PV pod manifest to Deployment include ReplicaSet in cluster 
│   ├── Using Functions
│   ├── Add tags to buckets storage.tf 
│   ├── Pointers
│   ├── Update deployment manifest, install Prometheus agent on all containers via daemonset, validate data is being ingested properly - validate
│   ├── Struct, Methods and Interfaces
│   ├── Cleanup Docker repo
│   ├── Conclusion
│   ├── Go script to provide VM name & IP upon Terraform creation in TXT file
│   └── Cleanup Python repo
├── GKE
│   ├── Configure service account IAM tagging in GCP 
│   ├── master.tf - update to install Prometheus agent on all Ubuntu guests, validate data is being ingested properly - validate
│   ├── Update container security in all pods via Deployment manifest
│   ├── Update compute.tf to inject RSA keys into VMs
│   └── Kubernetes Cluster: Install ProxMox Hypervisor
├── Helm
│   ├── Add HPA to Deployment manifest (K8)
│   ├── Create Grafana dashboard and cutover from Prometheus - ensure all data is being ingested properly 
│   ├── Add VPA to Deployment manifest (K8)
│   └── Remap cluster PVs to GCP buckets (K8)
├── CKA
│   ├── Update pod startup commands in Deployment manifest
│   ├── Containerize and add Ollama, nodeJS, mcp/jetbrains to Deployment manifest; add to monitoring (Prometheus/Grafana); connect to VMs (Unidirectional 1:1)
│   ├── Kubernetes Cluster: Provision and configure (4) Ubuntu Linux guests along with VSC, map to containers - Ollama, nodeJS, Go, mcp/jetbrains
│   └── GCP Infrastructure: Provision VM, install Terraform and configure main.tf
├── Go (Intermediate)
│   ├── Join Kubernetes SIG Networking
│   ├── Kubernetes Cluster: Provision and configure master and (3) worker node Kubernetes cluster on guests 
│   └── GCP Infrastructure: Using Terraform, provision and configure (4) VMs with each having Nginx, VSC and Chrome installed
├── GCP Cloud Digital Leader
│   ├── Kubernetes Cluster: Create, deploy and automate Go scripts
│   └── GCP Infrastructure: Configure DNS management for all VMs
├── PCA
│   ├── Kubernetes Cluster: Provision, test and configure Rook-ceph cluster
│   └── GCP Infrastructure: Connect, test and configure Kubernetes cluster to GCP storage bucket
├── Go (Advanced)
│   ├── Kubernetes Cluster: Provision test and configure containers for the following: Nginx, Prometheus, Python, Loki, Chromium/Ubuntu desktop, Anthropic MCP (Ollama), Redis, GitHub actions, MongoDB 
│   └── GCP Infrastructure: Configure Network Security rules
├── CGOA
│   ├── Kubernetes Cluster: Build out and configure Grafana dashboard for each cluster 
│   └── GCP Infrastructure: Provision and configure GKE cluster across all VMs (5 Node cluster - (1) master, (4) workers)
├── GCP ACE
│   ├── Kubernetes Cluster: Configure, test and deploy external reachability
│   └── GCP Infrastructure: Configure, test and deploy external reachability
├── CBA
│   └── TBD
├── CKS
│   └── TBD
├── ICA
│   └── TBD
├── CCA
│   └── TBD
