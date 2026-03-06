# Kubegrade

Kubegrade is a **Kubernetes platform focused on Day‑2 operations**: automating upgrades, troubleshooting, remediation and ongoing cluster maintenance, while keeping platform teams fully in control.

It connects directly to the Kubernetes API, so it can work with virtually any CNCF‑conformant cluster: managed (EKS/AKS/GKE), self‑hosted, on‑prem, or hybrid environments.


---

## What Kubegrade Does

- **Automated Kubernetes Ops Playbooks**  
  Encode multi‑step tasks (cluster upgrades, CNI/Ingress changes, operator rollouts, node pool rotations) as reusable workflows that can run safely across environments.  
  Dependency‑aware ordering makes sure the right components are drained, upgraded and validated in the correct sequence.

- **Drift & Health Monitoring for Clusters**  
  Continuously compares desired vs. actual state across clusters (versions, add‑ons, policies, configs) and surfaces risky drift before it breaks production.  
  Highlights which clusters, namespaces or workloads need attention, instead of forcing you to grep logs and dashboards manually.

- **Troubleshooting & Incident Workflows**  
  Correlates events, logs and metrics across namespaces and infrastructure layers to narrow down likely root causes.  
  Proposes concrete remediation steps (rollbacks, restarts, config changes, capacity tweaks) that can be executed via GitOps or CI/CD.

- **Cost & Capacity Optimization**  
  Analyzes resource usage and scheduling to find over‑provisioned workloads, idle clusters and noisy neighbors.  
  Suggests rightsizing and scaling changes that respect SLOs, not just raw CPU/Memory graphs.

---

## How It Fits in Your Stack

Kubegrade is designed to **augment** the stack you already have, not replace it.

- **Cluster Access & Topology**  
  - Connects directly to the Kubernetes API using service accounts and RBAC.  
  - Handles multi‑cluster and hybrid setups (cloud + on‑prem), as long as there is API connectivity and appropriate permissions.

- **GitOps & CI/CD Friendly**  
  - Works with Argo CD, Flux, Helm and Kustomize by creating or updating manifests instead of pushing ad‑hoc changes.  
  - Can open PRs / MRs in your Git repos or trigger pipelines rather than mutating clusters directly, so everything stays auditable.

- **Observability‑Aware**  
  - Uses the signals you already collect (metrics, logs, traces) to prioritize issues and validate that workflows actually improved things.  
  - Integrates with Prometheus/Grafana, Elastic/OpenSearch and other common stacks.

- **Guardrails & Governance**  
  - Respects RBAC and your existing security model; every action runs with the permissions you grant.  
  - Supports “propose‑only” modes (no direct writes), so platform teams remain the final decision‑makers.

---

## Tech & Platforms We Work With

### Kubernetes & Orchestrators
![Kubernetes](https://img.shields.io/badge/Kubernetes-326ce5?logo=kubernetes&logoColor=white)
![K3s](https://img.shields.io/badge/K3s-ffc61c?logo=kubernetes&logoColor=white)
![OpenShift](https://img.shields.io/badge/OpenShift-ee0000?logo=redhatopenshift&logoColor=white)

### Cloud Providers & Managed K8s
![AWS](https://img.shields.io/badge/AWS-232F3E?logo=amazonaws&logoColor=white)
![EKS](https://img.shields.io/badge/EKS-FF9900?logo=amazoneks&logoColor=white)
![Azure](https://img.shields.io/badge/Azure-0078D4?logo=microsoftazure&logoColor=white)
![AKS](https://img.shields.io/badge/AKS-0078D4?logo=azurekubernetesservice&logoColor=white)
![Google_Cloud](https://img.shields.io/badge/GCP-4285F4?logo=googlecloud&logoColor=white)
![GKE](https://img.shields.io/badge/GKE-34A853?logo=googlecloud&logoColor=white)
![On‑prem](https://img.shields.io/badge/On--prem_Kubernetes-444?logo=serverfault&logoColor=white)
![VMware_Tanzu](https://img.shields.io/badge/Tanzu-607078?logo=vmware&logoColor=white)

### GitOps, CI/CD & Packaging
![Argo CD](https://img.shields.io/badge/Argo_CD-F26722?logo=argo&logoColor=white)
![Flux](https://img.shields.io/badge/Flux_CD-009688?logo=flux&logoColor=white)
![Helm](https://img.shields.io/badge/Helm-0F1689?logo=helm&logoColor=white)
![Kustomize](https://img.shields.io/badge/Kustomize-7B42F6?logo=kubernetes&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2671E5?logo=githubactions&logoColor=white)
![GitLab CI](https://img.shields.io/badge/GitLab_CI-FC6D26?logo=gitlab&logoColor=white)
![Jenkins](https://img.shields.io/badge/Jenkins-D24939?logo=jenkins&logoColor=white)

### Observability & Telemetry
![Prometheus](https://img.shields.io/badge/Prometheus-E6522C?logo=prometheus&logoColor=white)
![Grafana](https://img.shields.io/badge/Grafana-F46800?logo=grafana&logoColor=white)
![OpenTelemetry](https://img.shields.io/badge/OpenTelemetry-000000?logo=opentelemetry&logoColor=white)
![Loki](https://img.shields.io/badge/Loki-4A8BDA?logo=grafana&logoColor=white)
![Elastic](https://img.shields.io/badge/Elastic_Stack-005571?logo=elasticstack&logoColor=white)
![OpenSearch](https://img.shields.io/badge/OpenSearch-005EB8?logo=opensearch&logoColor=white)

### Networking, Ingress & Service Mesh
![NGINX Ingress](https://img.shields.io/badge/NGINX_Ingress-009639?logo=nginx&logoColor=white)
![Traefik](https://img.shields.io/badge/Traefik-24A1C1?logo=traefikproxy&logoColor=white)
![Istio](https://img.shields.io/badge/Istio-466BB0?logo=istio&logoColor=white)
![Linkerd](https://img.shields.io/badge/Linkerd-2FCC71?logo=linkerd&logoColor=white)
![Envoy](https://img.shields.io/badge/Envoy_Proxy-AC4FC6?logo=envoyproxy&logoColor=white)
![Cilium](https://img.shields.io/badge/Cilium-1E3264?logo=cilium&logoColor=white)
![Calico](https://img.shields.io/badge/Calico-ED6A1F?logo=databricks&logoColor=white)

---

## Docs & Support

Documentation for Kubegrade will be **published soon**.

In the meantime, if you have any questions about features, integrations or your specific setup, please **reach out via the support form on our website**: `https://kubegrade.com/company/contact-us/`.
