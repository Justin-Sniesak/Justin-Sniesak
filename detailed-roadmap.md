```
├── Go 1
│   ├── v1 | v1
│   ├── *Attach GCP project to orginization and enable VM scanning | v1 | v1
│   ├── *Provision buckets/configure IAM using TF and configure IAM settings | v1 | v2 | v1
│   ├── *Configure Prometheus -> self monitoring -> configure dashboard -> expose externally | v1 | v2 | v1
│   ├── *Update all manifests to Deployment/ReplicaSet with rolling updates grouping pods per namespace | v1 | v2 | v1
│   ├── *Create and upload architectural diagram | v1 | v2 | v1
│   ├── *Remap cluster PVs to GCP buckets: Ensure end-toend connectivity between project and cluster | v1 | v2 | v1
│   ├── *Add tags to buckets storage.tf | v1 | v2 | v1
│   ├── *Configure Prometheus agent on all containers -> ensure data is being ingested and visualized on dadhboard for all pods (up/uptime/cpu/mem/etc) | v1 | v2 | v1
│   ├── *Update container security in all pods via Deployment manifest | PTR (3) | v1 | v2 | v1
│   ├── *Add Loki to monitoring and observability Deployment manifest -> map to CloudStorage for log collection -> validate functionality | v1 | v2 | v1
│   ├── *compute.tf: Change to Ubuntu desktop -> VSC install -> change all IP to ephimeral -> inject RSA keys -> Add VMs and convert bash script to Go | v1 | v2 | v1
│   ├── *Configure Grafana dashboard -> externally expose -> ensure all data from Prometheus is being ingested and visualized | v1 | v2 | v1
│   ├── *Update pod startup commands in Deployment manifest | v1 | v2 | v1
│   ├── *Install ProxMox Hypervisor -> install Terraform | v1 | v2 | v1
│   ├── *vpc.tf - Provision VPC with ephimeral IP assignment using TF and configure VPC Firewall rules | v1 | v2 | v1
│   ├── *Update deployment manifest -> install Prometheus agent on all containers via daemonset -> validate data is being ingested properly for all pods (argo/version)/cpu/mem/uptime | v1 | v2 | v1
│   └── *Add HPA to all Deployment manifest -> validate | v1 | v2 | v1
├── Helm
│   ├── *Convert all manifests into Helm charts -> upload to repo | v1 | v2 | v1
│   ├── *Deploy K8 cluster onto on-prem VMs | v1 | v2 | v1
│   ├── *Migrate all K8 from MK node to on-prem cluster -> validate all functionality including connectivity to GCP project -> update monitoring/observability -> confirm CloudStorage backup | v1 | v2 | v1
│   ├── *Add on-prem Hypervisor and Guests into monitoring/observability | v1 | v2 | v1
│   ├── *Provision, test and configure Rook for on-prem cluster | v1 | v2 | v1
│   └── *Add VPA to all Deployment manifest -> validate | v1 | v2 | v1
├── GKE
│   ├── *Update compute.tf to provision (4) Ubuntu desktop guests (Include VSC/Chrome) on-prem including injecting RSA keys -> expose to GCP project and confirm backing up to CloudStorage | v1 | v2 | v1
│   ├── *Deploy K8 cluster via GKE | v1 | v2 | v1
│   ├── *Add GKE cluster into monitoring/observability | v1 | v2 | v1
│   ├── *Configure Cloud DNS to include hypervisor, guests, on-prem cluster and GKE cluster | v1 | v2 | v1
│   ├── *Update vpc.tf to include firewall rules for GKE cluster and connectivity to on-prem cluster | v1 | v2 | v1
│   └── *IAM tagging audit for all SA in GCP project and with any connectivity to on-prem | v1 | v2 | v1
├── Go 2
│   ├── *Configure CloudBuild & Artifact Repository -> map to on-prem cluster -> -> validate CI/CD functionality with Helm charts | v1 | v2 | v1
│   ├── *Create pipeline repo for pod manifest/Argo | v1 | v2 | v1
│   ├── *Configure Argo -> test and confirm working -> internally expose on-prem and GCP Project -> validate GUI -> validate functionality -> Integrate with CloudBuild | v1 | v2 | v1
│   ├── *Create K8 secrets for MongoDB users and Argo SA | v1 | v2 | v1
│   ├── *Create pod/PV/PVC manifest for ARGO & MongoDB -> create SA for Argo -> Add to monitoring/observability -> map to CloudBuckets | v1 | v2 | v1
│   ├── *Write script for DB/Table/Users (Mongo) -> Validate functionality | v1 | v2 | v1
│   ├── Write, test, containerize and deploy (Go) app -> Add to monitoring/observability -> Add into CI/CD pipeline and test full functionality | v1 | v2 | v1
│   ├── Write, test, and automate Go scripts | v1 | v2 | v1
│   ├── *Write Deployment manifest: Python, Anthropic MCP, Redis, Ollama (AI Dev) -> push to GKE cluster -> add to monitoring/observability -> validate CI/CD functionality -> confirm writing to MongoDB | v1 | v2 | v1
│   ├── *Consolidate all mainfests into full scope deployment manifests -> push to repo and validate CI/CD | v1 | v2 | v1
│   ├── *Fully document entire stack full cloud/on-prem: GKE Cluster, On-Prem cluster, Hyper/Guests, monitoring, backend storage, CI/CD pipeline | v1 | v2 | v1
│   └── *Full functionality test of entire enterprise stack | v1 | v2 | v1
├── CKA
├── GCP Cloud Digital Leader
├── PCA
├── GCP ACE
├── CBA
├── CKS
├── ICA
└── CCA
