# 👨‍💻 Justin Sniesak  
**Senior Site Reliability Engineer | AI Infrastructure, Go, Cilium (eBPF), K8s | 5k+ Node Scale**  

---

## 🧩 About Me  
## Hi, I'm Justin 👋 

The Scale: Managed 5,000+ server fleets (RHEL/Ubuntu) and currently architecting 1,000-node hyperscale AI simulations.

Current Focus: Hardening the AI data plane using Go, Cilium (eBPF), and GPU-orchestration frameworks like Run:ai.

The Philosophy: Build for the mission. I prioritize zero-trust security, deep observability, and automation that eliminates "noise."

- **Languages:** Go (Golang), Bash, YAML 
- **Platform:** GPU Orchestration (H100), Run:ai, Kubernetes (GKE, kubeadm)
- **Networking & Security:** Cilium (Strict eBPF mode), Zero-Trust Policies, Hubble L7 Observability, DNS 
- **Systems:** Linux (RHEL, Ubuntu, Alpine), OrbStack, ESXi, Proxmox 
- **Cloud:** GCP, Hybrid Infrastructure, AWS 
- **IaC & CI/CD:** Terraform, Ansible (5k+ node fleet), ArgoCD, GitHub Actions

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

### 📚 Systematic Go
**Stack:** Golang, MacOS
- Structured Go learning repository: fundamentals → intermediate → advanced
- Demonstrates CLI tooling (tax/tip calculator with closures), structs, methods, and higher-order functions
- 🧾 Full logs, screenshots, and debugging notes across 30+ exercises

🔗 [View Repo](https://github.com/Justin-Sniesak/Golang)

---

### 🔐 Phase 1: High-Performance Networking & L7 Observability

**Stack: Kubernetes (kubeadm) · Cilium (eBPF) · Hubble · containerd · Helm**

- eBPF-Driven Networking: Replaced standard kube-proxy with Cilium in strict eBPF mode, eliminating iptables overhead and reducing latency for high-concurrency inter-node communication.

- L7 Traffic Auditing: Initialized Hubble agents for kernel-level visibility; verified zero-loss gRPC/HTTP traffic flows and established secure port-forwarding for real-time visualization.

- Identity-Based Policy: Traced East-West traffic within the Hubble UX to audit and confirm cryptographic identity-based network policy enforcement.

- 🧾 Validation: Fully documented with 6+ "receipt" screenshots proving connectivity suite success and API query-availability for external monitoring.

🔗 [View Repo](https://github.com/Justin-Sniesak/ai-infra-ops/tree/main/01_cluster_automation)

---

### 🧠 Phase 2: H100 GPU Simulation & Zero-Trust Hardening

**Stack: Kubernetes · Run:ai (Fake-GPU) · Cilium ZTP · Helm**

- Hardware Virtualization: Orchestrated 8x virtual NVIDIA H100 GPU nodes via Run:ai; applied targeted node labeling to synchronize inventory metadata and validate scheduler precision.

- Zero-Trust Egress (ZTP): Injected Cilium Network Policies to enforce a "deny-by-default" posture; verified kernel-level drops of unauthorized egress traffic to block data exfiltration and C2C communication.

- Stress-Test Validation: Executed cudatestpod deployments and intentionally over-requested resources to verify expected scheduler failure states and resource isolation.

- 🧾 Operational Audit: Conducted full egress security audits and documented successful container runtime initialization across the simulated fleet.

🔗 [View Repo](https://github.com/Justin-Sniesak/ai-infra-ops/tree/main/02_h100_cluster_simulation)

---

### 🚀 Hyperscale GPU Orchestration & Control Plane Hardening (Phase 3)

**Stack: Kubernetes (KWOK) · Bash · Linux Kernel Tuning · etcd · Helm · NVIDIA/AMD/Intel GPU Fleet**

- Engineered a 700+ line idempotent hydration engine to simulate a Tier-1 hyperscale environment: 2,000 nodes and 20,000 pods on a single workstation.

- Kernel-Level Hardening: Identified and mitigated host-level saturation by tuning sysctl and ulimit (1M+ file descriptors, 500k+ inotify watches) to maintain OS stability under extreme I/O.

- Control Plane Optimization: Resolved etcd "death spirals" by refactoring the quota-backend to 6Gi and tuning API Server mutation limits to survive the hydration of 20k concurrent objects.

- Heterogeneous Fleet Management: Automated the lifecycle of 20 distinct GPU architectures across NVIDIA, AMD, and Intel; built surgical cleanup logic to prevent ClusterRole and DeviceClass collisions during multi-vendor operator transitions.

- 🧾 Evidence-Based Engineering: Generated 40+ automated "receipts" (logs) validating node-level inventory and pod-level resource mapping across the entire 2k-node fleet.

🔗 [View Repo](https://github.com/Justin-Sniesak/ai-infra-ops/tree/main/03_hyperscale_GPU)

### All documentation and project sites listed here are automatically generated and deployed via custom GitHub Actions CI/CD pipelines. If it can be automated, it is.
