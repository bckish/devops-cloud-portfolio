# AI-driven engineering portfolio roadmap

This is an independent portfolio implementation plan inspired by the Wezva Technologies AI-Driven DevOps/MLOps/AIOps Projects BootCamp brief. It is not a claim of enrollment, certification, production employment, or the brochure's advertised performance metrics. Each deliverable must have its own code, reproducible test, and honest verification record.

The implementation follows a generic FinTech architecture: checkout UI, payment, ledger, notification and fraud-scoring services, separate build and deployment concerns, and shared infrastructure. Portfolio work is independently implemented; private course repository code and configurations are not redistributed.

## Seven capstones

| Capstone | Existing repository candidates | Next evidence milestone |
| --- | --- | --- |
| 1. Zero-touch DevSecOps delivery | [Order management](https://github.com/bckish/devsecops-order-management-app), [Jenkins/Argo CD](https://github.com/bckish/devsecops-eks-jenkins-argocd), [blue-green](https://github.com/bckish/kubernetes-blue-green-delivery) | Local CI, promotion gates and tested rollback; production deployment requires approval. |
| 2. Kubernetes microservice orchestration | [Go service](https://github.com/bckish/go-eks-github-actions-helm), [Java service](https://github.com/bckish/java-cicd-kubernetes), [Node three-tier](https://github.com/bckish/aws-eks-three-tier-platform) | Independent builds, readiness probes, scaling and local release verification. |
| 3. Zero-trust Kubernetes platform | [EKS least-privilege](https://github.com/bckish/eks-rbac-least-privilege), [EKS observability](https://github.com/bckish/eks-gitops-observability) | Namespace RBAC, policy enforcement, recovery exercise on a disposable cluster. |
| 4. Kubernetes diagnostic/remediation engine | [K8sGPT/Ollama](https://github.com/bckish/k8sgpt-ollama-cluster-triage) | Read-only diagnostics on synthetic incidents; human approval for remediation. |
| 5. Resource optimization | [AWS FinOps](https://github.com/bckish/aws-finops-automation), [EKS observability](https://github.com/bckish/eks-gitops-observability) | Offline telemetry forecast and bounded recommendations; no autonomous cloud resource edits. |
| 6. Multi-environment AWS IaC | [Terraform EKS](https://github.com/bckish/terraform-eks-platform), [AWS three-tier](https://github.com/bckish/terraform-aws-three-tier), [policy as code](https://github.com/bckish/terraform-policy-as-code) | Reusable modules, environment isolation and mocked Terraform plans without AWS apply. |
| 7. ML GitOps and telemetry | [MLOps foundations](https://github.com/bckish/Fundamentals-of-MLOps) | Reproducible synthetic dataset, model evaluation, local serving, artifact lineage and telemetry. |

## Coverage of numbered exercises

The ranges collectively cover exercises 1–65; candidate repositories are not evidence that each individual exercise is complete.

| Exercise IDs | Workstream | Existing starting points / gaps |
| --- | --- | --- |
| 1–2 | FinTech architecture and AWS network topology | Order-management architecture and Terraform three-tier; design a new synthetic FinTech architecture. |
| 3–11 | QA/prod compute, storage, CDN, HA, load balancing, networks, EKS, identities and filesystems | Terraform EKS, three-tier and RBAC; add independent reusable modules and mocked plans for missing components. |
| 12–16 | MongoDB Atlas, Valkey, RDS MySQL, registries and MSK | Kafka infrastructure and existing app data layers; cloud-specific managed services remain unverified. |
| 17–22 | Docker and CI for Node, Spring Boot and Go | Existing AWS three-tier, Java and Go repositories; strengthen language-specific CI and build evidence. |
| 23–27 | Environment promotion, GitOps and IaC CI | Jenkins/Argo CD, order management, Go/Java and Terraform policy as code; CI validation is distinct from delivery. |
| 28–30 | Jenkins backups, Docker housekeeping and golden images | Disaster recovery and Ansible infrastructure automation; use explicit dry-run and safe scoped cleanup. |
| 31–37 | Kubernetes deployment, frontend CDN, progressive release | Node/Java/Go repos and blue-green; Argo Rollouts and CDN need separate verification. |
| 38–41 | Vault, metrics, centralized logging and network policy | Azure GitOps, EKS observability, ELK pipeline, RBAC; validate tooling without live secrets. |
| 42–45 | K8sGPT, Alloy/Loki, OpenSearch, AI-assisted operations | K8sGPT/Ollama and logging; missing integrations need local examples and evaluation. |
| 46–53 | Scaling, upgrades, zero-touch platform, runtime detection, cost, chaos and backups | FinOps, observability, security scanning, disaster recovery; use only defensive detection and disposable exercises. |
| 54–60 | Managed data services and upgrade runbooks | Kafka and database migration; local substitutes and mocked cloud plans, not live AWS validation. |
| 61–65 | ML database, MLflow, serving, CI and telemetry | MLOps foundations; add lifecycle automation and measure actual model performance locally. |

## Definition of done

- Repository README: problem, architecture diagram, prerequisites, commands, known limitations and attribution.
- Working implementation and deterministic tests, plus reproducible local container or cluster examples where appropriate.
- CI with least privilege and no automatic paid-cloud operations. Cloud infrastructure is validated with mocks before any separately approved deployment.
- Resource budgets, safe local context selection and cleanup instructions.
- Evidence: date, tested revision, actual observations, and remaining gaps. No copied brochure ROI, uptime or MTTR figures.

## Suggested implementation order

1. Go microservice and blue-green delivery foundations.
2. Java microservice and CI/GitOps examples; integrate them with the existing Node and order-management projects.
3. Infrastructure modules and zero-trust controls.
4. AIOps read-only diagnostics and resource recommendation engine.
5. MLOps reproducible training, serving and monitoring.
6. Remaining specialized labs and cross-capstone evidence.
