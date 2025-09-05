```
├── Go
│   ├── Cleanup old Kubernetes repo | (3) DTV modules | purple pod manifest 1
│   ├── *Create pipeline repo for pod manifest/Argo | (3) DTV modules | purple pod manifest 2
│   ├── *Attach GCP project to orginization and enable VM scanning | (3) DTV modules | purple pod manifest 3
│   ├── *Create pod/PV/PVC manifest for ARGO & MongoDB; create SA for Argo |  (3) DTV modules | purple pod manifest 4
│   ├── *Provision buckets/configure IAM using TF and configure IAM settings | (3) DTV modules | purple pod manifest 5
│   ├── *Create K8 secrets for MongoDB users and Argo SA | (3) DTV modules | purple pod manifest 6
│   ├── *compute.tf - VSC install; change all IP to ephimeral; inject RSA keys; add new VMs to SSH script | (3) DTV modules | purple pod manifest 7
│   ├── *Write script for DB/Table/Users (Mongo & Argo)| (3) DTV modules | purple pod manifest 8
│   ├── *Create and upload architectural diagram | (3) DTV modules | purple pod manifest 9
│   ├── *Update all manifests to Deployment/ReplicaSet with rolling updates; group pods per use case | (3) DTV modules 
│   ├── *vpc.tf - Provision VPC with ephimeral IP assignment using TF and configure VPC Firewall rules | (3) OCF modules 
│   ├── *Configure Argo, test and confirm working, internally expose and validate GUI; confirm full CD functionality | (3) OCF modules 
│   ├── *Configure Prometheus; self monitoring; configure dashboard; expose externally | (3) OCF modules 
│   ├── *Consolidate all mainfests into deployment manifests including PV/PVC, ReplicaSets and Rolling updates, push to repo and confirm Argo pulls and applies | (3) OCF modules 
│   ├── *Update deployment manifest, install Prometheus agent on all containers via daemonset, validate data is being ingested properly for all pods: argo/cpu/mem/uptime | (3) OCF modules 
│   ├── *Write imperative run book for every step in GCP deployment, pipeline/argo & K8 cluster - attach to repo | Finish OCF 
│   ├── *Add tags to buckets storage.tf | ASM (3)
│   ├── *Configure Grafana dashboard, externally expose, ensure all data from Prometheus is being ingested and can be properly visualized | ASM (3)
│   ├── *Add Loki to monitoring and observability Deployment manifest, map to CloudStorage for log collection, validate functionality | Finish ASM
│   ├── Cleanup Docker repo | UF (3) 
│   ├── *Add HPA to all Deployment manifest, push to repo, confirm Argo pulls and applies | UF (3)
│   ├── Cleanup Python repo | UF (3)
│   ├── *Add VPA to all Deployment manifest, push to repo, confirm Argo pulls and applies | UF (3)
│   ├── *Update pod startup commands in Deployment manifest | Finish UF
│   ├── *Remap cluster PVs to GCP buckets (Backend Storage) | PTR (3) 
│   ├── *Update container security in all pods via Deployment manifest | PTR (3)
│   ├── Finish Pointers
│   ├── Struct, Methods and Interfaces
│   └── Conclusion
├── Helm
│   └── *Convert all manifests into Helm charts, upload to repo, confirm CD functionality
├── GKE
│   ├── *Deploy K8 cluster via GKE
│   ├── *IAM tagging audit for all SA in GCP project and with any connectivity to on-prem
│   ├── *Configure CloudBuild, map to on-prem cluster, integrate with Argo, confirm full CI/CD functionality with Helm charts: CloudBuild -> ArgoCD
│   ├── *Install ProxMox Hypervisor, install Terraform
│   ├── *Update compute.tf to provision (4) Ubuntu desktop guests (Include VSC/Chrome) on-prem including injecting RSA keys; expose to GCP project and confirm backing up to CloudStorage
│   ├── *Deploy K8 cluster onto on-prem VMs
│   ├── *Migrate all K8 from MK node to on-prem cluster - confirm all functionality including connectivity to GCP project and GKE cluster, update monitoring/observability, confirm CloudStorage backup
│   ├── *Add GKE cluster into monitoring/observability
│   ├── *Update vpc.tf to include firewall rules for GKE cluster and connectivity to on-prem cluster
│   ├── *Add on-prem Hypervisor and Guests into monitoring/observability
│   ├── *Configure Cloud DNS to include hypervisor, guests, on-prem cluster and GKE cluster
│   ├── *Write Deployment manifest: Python, Anthropic MCP, Redis, Ollama (AI Dev) - push to GKE cluster - add to monitoring/observability - confirm CI/CD functionality - confirm writing to MongoDB
│   ├── *Provision, test and configure Rook for on-prem cluster
│   └── *Full functionality test of entire enterprise stack
├── CKA
├── Go (Intermediate)
├── GCP Cloud Digital Leader
├── PCA
├── Go (Advanced)
├── GCP ACE
├── CBA
├── CKS
├── ICA
└── CCA
