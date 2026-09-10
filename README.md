# Amine JAFJAF

**Technical Project Leader — Reliable Systems, Infrastructure & Digital Trust**

Je relie ingénierie des infrastructures, automatisation et pilotage technique. Mes sujets : IT Production, DevOps, SRE, Python, Ansible, Infrastructure as Code, TLS, PKI et gestion des identités.

Mon site personnel rassemble des articles et des projets, avec des sources techniques et des limites explicites. Les exemples pédagogiques ne sont pas présentés comme des résultats clients.

- [Site personnel](https://aminejafjaf.com/)
- [Profil et expertise](https://aminejafjaf.com/about)
- [Articles techniques](https://aminejafjaf.com/articles)
- [Projets](https://aminejafjaf.com/projects)

## Quelques lectures

Un exemple de code : [TLS Endpoint Check](https://github.com/aminejafjaf-wq/tls-endpoint-check), un laboratoire Python avec des tests TLS locaux pour contrôler identité, confiance et expiration d’un certificat.

- [Automatisation des certificats TLS](https://aminejafjaf.com/articles/automatisation-certificats-tls)
- [PKI et chaîne de confiance](https://aminejafjaf.com/articles/pki-chaine-de-confiance)
- [Infrastructure as Code : avantages et limites](https://aminejafjaf.com/articles/infrastructure-as-code)
- [DevOps, SRE et IT Production](https://aminejafjaf.com/articles/devops-sre-it-production)

Ces publications sont personnelles. Elles n'engagent aucun employeur et ne reproduisent pas d'architecture confidentielle.

<!-- engineering-portfolio:start -->
## Engineering portfolio

Twenty independent projects, organized around reliable infrastructure and digital trust. Each repository includes runnable code, synthetic examples, tests, CI, an MIT license, architecture notes and explicit limitations. These are local demonstrators and reference implementations; no production adoption is claimed.

### TLS, certificats et PKI

| Project | Purpose | Technologies | Skills | Maturity / validation |
|---|---|---|---|---|
| [tls-expiry-monitor](https://github.com/aminejafjaf-wq/tls-expiry-monitor) | Concurrent verified TLS inventory monitoring | Python 3.12, cryptography | TLS, deadlines, supervision | Outil de référence testé · [CI](https://github.com/aminejafjaf-wq/tls-expiry-monitor/actions/runs/34519862109) |
| [certificate-inventory-api](https://github.com/aminejafjaf-wq/certificate-inventory-api) | Persistent searchable certificate ownership inventory | Python 3.12, FastAPI, SQLite | API design, validation, SQLite | Outil de référence testé · [CI](https://github.com/aminejafjaf-wq/certificate-inventory-api/actions/runs/34519873135) |
| [csr-policy-validator](https://github.com/aminejafjaf-wq/csr-policy-validator) | Enforce an explicit certificate request policy | Python 3.12, cryptography | PKCS#10, SAN, key and extension policies | Outil de référence testé · [CI](https://github.com/aminejafjaf-wq/csr-policy-validator/actions/runs/34521200173) |
| [pki-lab](https://github.com/aminejafjaf-wq/pki-lab) | Build a local trust chain and prove revocation | Python 3.12, cryptography, OpenSSL | CA constraints, EKU, CRL, OpenSSL | Laboratoire testé · [CI](https://github.com/aminejafjaf-wq/pki-lab/actions/runs/34519884927) |
| [mtls-service-lab](https://github.com/aminejafjaf-wq/mtls-service-lab) | Demonstrate authenticated client/server transport | Python 3.12, cryptography, Docker Compose | mTLS, application identity, Compose | Laboratoire testé · [CI](https://github.com/aminejafjaf-wq/mtls-service-lab/actions/runs/34521212950) |
| [ocsp-crl-checker](https://github.com/aminejafjaf-wq/ocsp-crl-checker) | Verify signed offline revocation evidence | Python 3.12, cryptography | X.509 revocation, freshness, issuer binding | Outil de référence testé · [CI](https://github.com/aminejafjaf-wq/ocsp-crl-checker/actions/runs/34521224926) |
| [certificate-lifecycle-orchestrator](https://github.com/aminejafjaf-wq/certificate-lifecycle-orchestrator) | Model renewal and revocation with a durable audit trail | Python 3.12, SQLite | State machines, idempotency, concurrency | Simulateur testé · [CI](https://github.com/aminejafjaf-wq/certificate-lifecycle-orchestrator/actions/runs/34521236829) |
| [ansible-tls-deployer](https://github.com/aminejafjaf-wq/ansible-tls-deployer) | Deploy a matching TLS pair with rollback | Python 3.12, cryptography, Ansible, Docker | Ansible, idempotence, file modes, recovery | Laboratoire testé · [CI](https://github.com/aminejafjaf-wq/ansible-tls-deployer/actions/runs/34519897518) |
| [nginx-tls-hardening-lab](https://github.com/aminejafjaf-wq/nginx-tls-hardening-lab) | Compare Nginx TLS profiles without public infrastructure | Python 3.12, cryptography, Docker Compose, Nginx | TLS negotiation, headers, compatibility | Laboratoire testé · [CI](https://github.com/aminejafjaf-wq/nginx-tls-hardening-lab/actions/runs/34521246881) |
| [tls-configuration-auditor](https://github.com/aminejafjaf-wq/tls-configuration-auditor) | Explain findings from a scoped TLS configuration audit | Python 3.12, cryptography, OpenSSL | Protocol probes, Nginx configuration analysis | Outil de référence testé · [CI](https://github.com/aminejafjaf-wq/tls-configuration-auditor/actions/runs/34521259881) |

### Infrastructure, DevOps et automatisation

| Project | Purpose | Technologies | Skills | Maturity / validation |
|---|---|---|---|---|
| [infrastructure-health-check](https://github.com/aminejafjaf-wq/infrastructure-health-check) | Run typed DNS/TCP/HTTP/TLS health probes | Python 3.12, YAML | Modular probes, timing, error isolation | Outil de référence testé · [CI](https://github.com/aminejafjaf-wq/infrastructure-health-check/actions/runs/34519939317) |
| [infra-drift-detector](https://github.com/aminejafjaf-wq/infra-drift-detector) | Compare desired and observed structured state | Python 3.12, YAML | JSON pointers, drift policies, CI | Outil de référence testé · [CI](https://github.com/aminejafjaf-wq/infra-drift-detector/actions/runs/34521746655) |
| [configuration-compliance-auditor](https://github.com/aminejafjaf-wq/configuration-compliance-auditor) | Evaluate configuration rules with dated exceptions | Python 3.12, YAML | Policy validation, exception governance | Outil de référence testé · [CI](https://github.com/aminejafjaf-wq/configuration-compliance-auditor/actions/runs/34521761898) |
| [gitops-environment-promoter](https://github.com/aminejafjaf-wq/gitops-environment-promoter) | Promote immutable versions with predecessor checks | Python 3.12 | GitOps manifests, audit, logical rollback | Simulateur testé · [CI](https://github.com/aminejafjaf-wq/gitops-environment-promoter/actions/runs/34521772619) |
| [deployment-readiness-gate](https://github.com/aminejafjaf-wq/deployment-readiness-gate) | Explain release readiness including change windows | Python 3.12 | Fail-closed governance, evidence, UTC | Outil de référence testé · [CI](https://github.com/aminejafjaf-wq/deployment-readiness-gate/actions/runs/34519921941) |
| [automation-control-plane](https://github.com/aminejafjaf-wq/automation-control-plane) | Execute only catalogued simulated operations | Python 3.12, SQLite | RBAC, parameter validation, audit, idempotency | Simulateur testé · [CI](https://github.com/aminejafjaf-wq/automation-control-plane/actions/runs/34521787841) |

### SRE, fiabilité et résilience

| Project | Purpose | Technologies | Skills | Maturity / validation |
|---|---|---|---|---|
| [sre-slo-toolkit](https://github.com/aminejafjaf-wq/sre-slo-toolkit) | Calculate request-based SLO budgets and burn rates | Python 3.12 | SLI, error budgets, window aggregation | Outil de référence testé · [CI](https://github.com/aminejafjaf-wq/sre-slo-toolkit/actions/runs/34519934902) |
| [reliability-game-day-simulator](https://github.com/aminejafjaf-wq/reliability-game-day-simulator) | Compare resilience strategies against seeded faults | Python 3.12 | Retries, deadlines, circuit breakers | Simulateur testé · [CI](https://github.com/aminejafjaf-wq/reliability-game-day-simulator/actions/runs/34521275199) |
| [incident-runbook-automation](https://github.com/aminejafjaf-wq/incident-runbook-automation) | Resume a safe declarative incident runbook | Python 3.12, YAML | Preconditions, checkpoints, audit, recovery | Simulateur testé · [CI](https://github.com/aminejafjaf-wq/incident-runbook-automation/actions/runs/34521288962) |

### Pilotage et gouvernance technique

| Project | Purpose | Technologies | Skills | Maturity / validation |
|---|---|---|---|---|
| [technical-project-governance-kit](https://github.com/aminejafjaf-wq/technical-project-governance-kit) | Initialize and validate a project governance workspace | Python 3.12 | RACI, RAID, dependencies, readiness, risk scoring | Outil de référence testé · [CI](https://github.com/aminejafjaf-wq/technical-project-governance-kit/actions/runs/34519946763) |

Start with **pki-lab**, **ansible-tls-deployer**, **certificate-inventory-api**, **sre-slo-toolkit**, **deployment-readiness-gate** or **technical-project-governance-kit** for a cross-section of the portfolio.

All commits reflect the actual development work. Local keys are generated on demand; no private lab keys or employer data are published. [Browse the French project guide](https://aminejafjaf.com/projects).
<!-- engineering-portfolio:end -->
