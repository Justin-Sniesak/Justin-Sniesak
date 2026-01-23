# 👨‍💻 Justin Sniesak  
**Platform & Site Reliability Engineer | Cloud-Native | Kubernetes | Terraform | Ansible | Linux (Ubuntu/RHEL) | Cilium | Go | GCP | Automation | CI/CD Pipelines**  

---

## 🧩 About Me  
## Hi, I'm Justin 👋 

Senior SRE & Platform Engineer specializing in high-scale infrastructure and deterministic automation.

Languages: Go, Bash, YAML

Platforms: Kubernetes (GKE, kubeadm), Linux (RHEL, Ubuntu, Alpine), ESXi

Cloud: GCP

Monitoring/Observability: Prometheus, Grafana, Node Exporter, DataDog

Networking: Cilium, Zero-Trust Policies, Hubble, DNS (Infoblox)

IaC: Terraform, Ansible (Fleet scale: 5,000+ nodes), ArgoCD, GitHub Actions

Background: Senior Incident Commander (FinTech) & Navy Veteran.

---

## ⚙️ Featured Projects

### 🧩 ArgoCD + GKE CI/CD Pipeline Lab
Stack: Go · Docker · GitHub Actions · GCP Artifact Registry · GKE · ArgoCD
- Built a complete end-to-end GitOps CI/CD pipeline from scratch — Go code to production on GKE in 7 hours.
- Implemented GitHub Actions for automated builds, GCP Artifact Registry for image management, and ArgoCD for continuous delivery.
- Validated full deployment lifecycle including intentional pod failures, permissions hardening, and service account RBAC.
- 🧾 Fully documented with architecture diagram, runbook, and 50+ screenshots.

🔗 [View Repo](https://justin-sniesak.github.io/GCP-Argo-GHA-Pipeline/)

---

### 🧠 Platform Engineering Lab  
Stack: Kubernetes (Minikube), Terraform, Prometheus, GCP, ProxMox   
- Built multi-namespace Kubernetes environment in Minikube on bare-metal Ubuntu, integrated with GCP and ProxMox for hybrid operations. Implemented Istio, RBAC, and Zero-Trust controls with full observability.
- ⏱️ Terraform cut provisioning from 6 h → 5 m | 📊 MTTR reduced ~50% | 🧾 Fully documented ops logs   

🔗 [View Repo](https://github.com/Justin-Sniesak/Platform-Engineering-Lab)

---

### ☁️ AWS Hybrid Cloud + DataDog Migration  
**Stack:** AWS, ProxMox, Terraform, WireGuard, DataDog, Prometheus
- Deployed site-to-site VPN and migrated observability from Prometheus → DataDog in 13 hours.  
- 6 production dashboards, 10+ documented troubleshooting events, and enforced IAM least privilege.  

🔗 [View Repo](https://github.com/Justin-Sniesak/AWS-HybridCloud-Prometheus-DataDog-Migration)

---

### 🔄 Go + Docker + GitHub Actions CI/CD  
**Stack:** Go, Docker, GitHub Actions, GCP Artifact Registry  
- Containerized a Go app and built CI/CD from build → test → deploy.  
- Automated tagging and artifact push to GCP with fully documented failures and fixes.  

🔗 [View Repo](https://justin-sniesak.github.io/go-docker-githubactions-pipeline/)

---

### 🔐 Kubernetes Cilium Zero-Trust Networking 
**Stack**: Kubernetes (kubeadm) · Cilium · Hubble · containerd · Helm · Parallels (ARM)
- Built a three-node Kubernetes cluster from scratch using kubeadm and containerd on ARM-based VMs.
- Replaced kube-proxy with Cilium and implemented identity-based, namespace-scoped zero-trust network policies.
- Designed explicit ingress and egress controls for client, edge, and backend workloads, including DNS allowlisting.
- Validated policy enforcement at the dataplane using cilium-dbg and Hubble UI/CLI, including dropped traffic analysis.
- Troubleshot real-world failure modes including container runtime incompatibilities, CNI routing mode mismatches, and silent namespace-scoping errors.
- Fully documented with architecture diagram, detailed ops log, and enforcement validation screenshots.

🔗 [View Repo](https://github.com/Justin-Sniesak/kubernetes-cilium-zerotrust-architecture)

---

### 📚 Systematic Go Learning
**Stack:** Golang, MacOS
- Structured Go learning repository: fundamentals → intermediate → advanced
- Demonstrates CLI tooling (tax/tip calculator with closures), structs, methods, and higher-order functions
🧾 Full logs, screenshots, and debugging notes across 30+ exercises

🔗 [View Repo](https://github.com/Justin-Sniesak/Golang)

---

- All documentation and project sites listed here are automatically generated and deployed via custom GitHub Actions CI/CD pipelines. If it can be automated, it is.
