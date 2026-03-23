# 👨‍💻 Justin Sniesak  
**Senior Site Reliability Engineer | AI Infrastructure, Go, Cilium (eBPF), K8s | 5k+ Node Scale**  

---

## 🧩 About Me  
## Hi, I'm Justin 👋 

Infrastructure engineer focused on large-scale systems, Kubernetes control plane behavior, and compute infrastructure under real-world conditions.

Experience operating 5,000+ node production environments and building hyperscale simulation platforms (2,000 nodes / 20,000 pods) to validate system behavior under load.

Current work centers on eBPF-based networking (Cilium), GPU orchestration, and failure-aware infrastructure automation — with an emphasis on verifying behavior at the dataplane and control plane, not assuming it.

- **Languages:** Go (Golang), Bash, YAML 
- **Platform:** GPU Orchestration, Run:ai, Kubernetes (GKE, kubeadm, KWOK)
- **Networking & Security:** Cilium (Strict eBPF mode), Zero-Trust Policies, Hubble L7 Observability, DNS 
- **Systems:** Linux (RHEL, Ubuntu, Alpine), OrbStack
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

### 🚀 Phase 3: Hyperscale GPU Orchestration & Control Plane Hardening 

**Stack: Kubernetes (KWOK) · Bash · Linux Kernel Tuning · etcd · Helm · NVIDIA/AMD/Intel GPU Fleet**

- Engineered a 700+ line idempotent hydration engine to simulate a Tier-1 hyperscale environment: 2,000 nodes and 20,000 pods on a single workstation.

- Kernel-Level Hardening: Identified and mitigated host-level saturation by tuning sysctl and ulimit (1M+ file descriptors, 500k+ inotify watches) to maintain OS stability under extreme I/O.

- Control Plane Optimization: Resolved etcd "death spirals" by refactoring the quota-backend to 6Gi and tuning API Server mutation limits to survive the hydration of 20k concurrent objects.

- Heterogeneous Fleet Management: Automated the lifecycle of 20 distinct GPU architectures across NVIDIA, AMD, and Intel; built surgical cleanup logic to prevent ClusterRole and DeviceClass collisions during multi-vendor operator transitions.

- 🧾 Evidence-Based Engineering: Generated 40+ automated "receipts" (logs) validating node-level inventory and pod-level resource mapping across the entire 2k-node fleet.

🔗 [View Repo](https://github.com/Justin-Sniesak/ai-infra-ops/tree/main/03_hyperscale_GPU)

### All documentation and project sites listed here are automatically generated and deployed via custom GitHub Actions CI/CD pipelines. If it can be automated, it is.
