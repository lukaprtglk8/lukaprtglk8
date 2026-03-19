# Kubegrade

Kubegrade is a **Kubernetes platform focused on Day‑2 operations**: automating upgrades, troubleshooting, remediation and ongoing cluster maintenance, while keeping platform teams fully in control.

It connects directly to the Kubernetes API, so it can work with virtually any CNCF‑conformant cluster: managed (EKS/AKS/GKE), self‑hosted, on‑prem, or hybrid environments.

---

## What Kubegrade Does

- **Automated Kubernetes Ops Playbooks**  
  Encode multi‑step tasks (cluster upgrades, CNI/Ingress changes, operator rollouts, node pool rotations) as reusable workflows that can run safely across environments.  
  Dependency‑aware ordering makes sure the right components are drained, upgraded and validated in the correct sequence.

- **Drift & Health Monitoring for Clusters**  
  Continuously compares desired vs actual state across clusters (versions, add‑ons, policies, configs) and surfaces risky drift before it breaks production.  
  Highlights which clusters, namespaces or workloads need attention, instead of forcing you to grep logs and dashboards manually.

- **Troubleshooting & Incident Workflows**  
  Correlates events, logs and metrics across namespaces and infrastructure layers to narrow down likely root causes.  
  Proposes concrete remediation steps (rollbacks, restarts, config changes, capacity tweaks) that can be executed via GitOps or CI/CD.

- **Alert Sorting & Signal Management**  
  Ingests alerts from your existing observability stack, de‑duplicates and groups them, and surfaces the ones that actually impact services.  
  Enriches signals with cluster context and recent changes so on‑call engineers can act quickly instead of hunting for data.

- **Fleet & Policy Management**  
  Provides multi‑cluster visibility, GitOps‑driven policy enforcement and standardized remediation patterns across your entire fleet.  
  Ensures that security baselines and platform guardrails are applied consistently, with every fix going through version‑controlled change requests.

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
  - Uses the signals you already collect (metrics, logs, traces, alerts) to prioritize issues and validate that workflows actually improved things.  
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
![GCP](https://img.shields.io/badge/GCP-4285F4?logo=googlecloud&logoColor=white)
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

### Observability & Alerting
![Prometheus](https://img.shields.io/badge/Prometheus-E6522C?logo=prometheus&logoColor=white)
![Grafana](https://img.shields.io/badge/Grafana-F46800?logo=grafana&logoColor=white)
![OpenTelemetry](https://img.shields.io/badge/OpenTelemetry-000000?logo=opentelemetry&logoColor=white)
![Loki](https://img.shields.io/badge/Loki-4A8BDA?logo=grafana&logoColor=white)
![Elastic](https://img.shields.io/badge/Elastic_Stack-005571?logo=elasticstack&logoColor=white)
![OpenSearch](https://img.shields.io/badge/OpenSearch-005EB8?logo=opensearch&logoColor=white)
![PagerDuty](https://img.shields.io/badge/PagerDuty-06AC38?logo=pagerduty&logoColor=white)
![Slack](https://img.shields.io/badge/Slack-4A154B?logo=slack&logoColor=white)

---

## Docs & Getting Started

Product documentation is being consolidated and will be **published soon**.

In the meantime:

- Website & product overview: `https://kubegrade.com`  
- To discuss your setup or request a demo, contact us via the support form: `https://kubegrade.com/company/contact-us/`.
