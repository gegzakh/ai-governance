# AI Governance Platform for Banks — Business Requirements

**Document type:** Business Requirements Document (BRD)  
**Target state:** Production enterprise platform, not the public demonstration  
**Status:** Baseline for discovery, estimation, legal validation, and phased delivery  
**Version:** 1.0 — 3 September 2026

## 1. Executive summary

The AI Governance Platform enables a bank to discover, register, classify, approve, monitor, and evidence every AI system and use case across its lifecycle. It converts policy and regulation into a controlled operating process that connects business ownership, model risk, privacy, security, compliance, legal review, third-party oversight, human accountability, performance monitoring, incidents, and change management.

The production product must replace the demo's synthetic records and browser storage with secure enterprise persistence, configurable regulatory/policy mappings, multi-stage workflows, evidence management, integrations, continuous monitoring, and defensible audit history.

## 2. Problems to solve

1. Banks do not have a single, current inventory of predictive AI, machine learning, generative AI, embedded vendor AI, or automated-decision use cases.
2. Teams interpret policies differently and governance starts too late, creating delivery delays and inconsistent controls.
3. Inherent risk, residual risk, regulatory role, prohibited-use screening, and materiality are assessed manually and cannot be reproduced reliably.
4. Evidence is scattered across tickets, documents, model registries, vendor files, test tools, and email approvals.
5. Provider, model, data, prompt, version, and deployment changes can occur without appropriate reassessment.
6. Human oversight, transparency, fairness, privacy, security, resilience, and customer-impact controls are difficult to prove continuously.
7. Third-party model dependencies and concentration risks are poorly understood.
8. Executives, risk committees, auditors, and regulators lack a consistent view of exposure, findings, incidents, and overdue actions.

## 3. Product vision

Create the bank's accountable control plane for AI: every use case is known, owned, risk-classified, approved for a defined purpose, supported by evidence, monitored against control obligations, and re-evaluated when risk or implementation changes.

## 4. Business objectives and success measures

| Objective | Target measure after rollout |
|---|---|
| Establish complete inventory | At least 98% of known production AI use cases registered and owner-attested |
| Shift governance left | 100% of material AI initiatives screened before production procurement/development approval |
| Standardize risk decisions | 100% of classifications reproducible from a versioned questionnaire and ruleset |
| Improve control readiness | No production high-risk use case without mandatory approvals and accepted evidence/exception |
| Control lifecycle change | All material model, provider, data, purpose, autonomy, or deployment changes trigger reassessment |
| Reduce manual evidence work | 60% reduction in time to prepare AI governance committee/audit evidence packs |
| Improve oversight | All overdue findings, monitoring breaches, incidents, and expiring exceptions have an owner and escalation |

Exact thresholds are configurable and must be approved by the bank's policy, legal, compliance, and model-risk functions.

## 5. Regulatory and policy baseline

The product must support configurable mappings rather than claim automatic legal compliance. The baseline includes:

- EU AI Act risk categories, prohibited-practice screening, transparency, high-risk obligations, deployer/provider responsibilities, human oversight, documentation, logging, robustness, accuracy, cybersecurity, monitoring, and incident handling.
- Banking model-risk, operational-risk, outsourcing/third-party, data protection, information security, records-management, consumer-protection, conduct, and product-governance policies.
- Institution-specific policies and jurisdictional overlays.
- Optional control mappings to recognized standards/frameworks such as ISO/IEC 42001, ISO/IEC 23894, NIST AI RMF, privacy standards, and internal control catalogs.

Legal applicability, regulatory role, deadlines, and final classification remain accountable human decisions. The EU AI Act uses a risk-based approach and requires strict controls for applicable high-risk systems; obligations and timelines continue to evolve, so the platform must version its regulatory content.

## 6. Stakeholders and personas

| Persona | Primary need |
|---|---|
| AI/use-case owner | Register an initiative, understand obligations, submit evidence, and maintain approval |
| AI governance office | Policy implementation, inventory, triage, workflow, oversight, and committee reporting |
| Model risk management | Independent validation, limitations, performance, drift, and model lifecycle |
| Compliance and legal | Regulatory applicability, prohibited uses, transparency, conduct, and legal decisions |
| Privacy/DPO | Data purpose, lawful basis, DPIA, minimization, retention, and data-subject impacts |
| Security and resilience | Threat modeling, supplier risk, abuse controls, incident response, continuity, and concentration |
| Data/ML engineering | Technical inventory, datasets, evaluations, versions, deployments, and monitoring evidence |
| Procurement/vendor management | Provider due diligence, contract controls, subcontractors, regions, and exit strategy |
| Business/customer-risk reviewer | Customer outcomes, fairness, explainability, complaints, human review, and overrides |
| Executive/risk committee | Portfolio exposure, decisions, exceptions, incidents, and readiness |
| Auditor/regulator | Immutable history, decisions, evidence, testing, monitoring, and accountability |

## 7. Business scope

### 7.1 In scope

- Discovery and inventory of internally built, third-party, embedded, shadow, and general-purpose AI usage.
- Intake, prohibited-practice screening, risk classification, applicability, and regulatory-role assessment.
- Configurable governance pathways by jurisdiction, entity, use case, risk, technology, and lifecycle stage.
- Multidisciplinary approvals, segregation of duties, conditions, exceptions, and committee decisions.
- Control library, evidence requests, testing, validation, gaps, remediation, and attestations.
- Provider/model/dataset/prompt/application/deployment lineage and version/change governance.
- Human oversight, transparency, customer-impact, fairness, explainability, privacy, security, resilience, and quality controls.
- Production monitoring, incidents, complaints, performance/drift, serious-event escalation, and reassessment.
- Third-party AI inventory, due diligence, contractual obligations, data regions, concentration, and exit readiness.
- Dashboards, reporting, regulatory/audit evidence packs, notifications, APIs, and integrations.
- Permission-aware AI assistance for intake, gap analysis, policy mapping, and evidence summarization with citations and human approval.

### 7.2 Out of scope for initial production release

- Replacing model development, experiment tracking, data catalogs, SIEM, ITSM, procurement, or document-management platforms.
- Automatically approving/rejecting a use case or making final legal/regulatory determinations.
- Autonomous suspension of production AI without a pre-approved safety policy and accountable control.
- Treating vendor claims or generated documentation as verified evidence.

## 8. Required business capabilities

1. **AI inventory and discovery** across business units, vendors, code, cloud, and model platforms.
2. **Risk and applicability assessment** using versioned questionnaires/rules and human sign-off.
3. **Governance workflow** with parallel/sequential reviews, conditions, exceptions, and expiry.
4. **Control and evidence management** mapped to policy, regulation, risk, system, and lifecycle stage.
5. **Model/system lineage** linking purpose, owner, provider, model, dataset, prompt, application, deployment, and user population.
6. **Independent validation and evaluation** for quality, robustness, fairness, explainability, security, privacy, and human oversight.
7. **Continuous monitoring** of approved use, performance, drift, incidents, complaints, overrides, and control health.
8. **Third-party oversight** for providers, contracts, subcontractors, data use, regions, concentration, and exit.
9. **Change governance** so material changes reopen affected obligations and approvals.
10. **Portfolio oversight** with exposure, readiness, overdue work, trends, and board/regulatory reporting.

## 9. Core business processes

### 9.1 Intake and triage

The use-case owner registers the intended purpose, users, affected persons, decisions, autonomy, data, provider/model, jurisdictions, critical processes, and deployment plan. The platform screens for prohibited uses, assigns provisional risk/applicability, identifies the bank's role, and routes the case to required reviewers.

### 9.2 Assessment and approval

Reviewers complete domain assessments, request evidence, record findings, and validate mandatory controls. The accountable authority approves, conditionally approves, rejects, pauses, or grants a time-bound exception. Approval is limited to the recorded purpose, model/system version, population, data, geography, channel, and operating constraints.

### 9.3 Deployment and ongoing oversight

Only an approved configuration may pass the configured production gate. Monitoring data, evaluations, complaints, overrides, incidents, and changes are linked continuously. Threshold breaches or material changes create findings, incidents, or mandatory reassessment.

### 9.4 Retirement

The owner records end of use, disables integrations, preserves required records, confirms data/model disposal obligations, transfers unresolved issues, and receives closure approval.

## 10. Business rules

1. Every AI use case must have an accountable business owner and technical owner.
2. Approval is purpose-, scope-, jurisdiction-, population-, model-, provider-, data-, version-, and deployment-specific.
3. Prohibited-practice screening is mandatory before further approval and must be re-run after relevant regulatory or purpose changes.
4. Risk classification must be explainable, reproducible, versioned, and independently overridable only with rationale and authority.
5. A use case cannot enter production when mandatory approvals/evidence are missing, expired, rejected, or subject to a blocking finding unless an authorized exception explicitly permits it.
6. Material changes must trigger impact analysis and reopen only the affected assessments/controls plus any configured mandatory reviews.
7. AI-generated content is draft support, not evidence, until an authorized person validates it.
8. Monitoring thresholds, incidents, serious-event criteria, customer harm indicators, and escalation paths must be configurable.
9. Human oversight must specify decision rights, competence, information, time, override, escalation, and fallback—not just a named reviewer.
10. Audit and evidence records for approved/rejected decisions must be immutable under the applicable retention schedule.

## 11. Security, privacy, and data outcomes

- SSO/MFA, least privilege, segregation of duties, privileged-access review, and entity/data-classification controls.
- Encryption, tenant/entity isolation, approved data regions, secrets management, and tamper-evident audit.
- Data minimization, purpose limitation, DPIA linkage, retention/deletion, data-subject rights, and sensitive-field protection.
- No provider training on bank inputs/outputs unless explicitly approved and contractually controlled.
- Prompt/output redaction, content controls, provider allow-lists, usage telemetry, and emergency disablement.
- Secure evidence storage with malware scanning, legal hold, watermark/export controls where required.

## 12. Risks and mitigations

| Risk | Required mitigation |
|---|---|
| Inventory is incomplete | Discovery integrations, attestations, procurement/technology gates, and shadow-AI reporting |
| Governance becomes a bottleneck | Risk-based workflow, reusable controls, templates, parallel review, SLA/escalation |
| False compliance confidence | Configurable content, legal sign-off, effective-date/version visibility, and disclaimers |
| Evidence is low quality | Evidence criteria, source/owner/date, independent validation, expiry, and sampling |
| Model/provider changes bypass review | Technical lineage, deployment gates, webhooks, material-change rules |
| Sensitive data leaks to AI providers | Redaction, allow-lists, DLP, regional routing, contract controls, and monitoring |
| Automated score is treated as final | Explainability, human override with rationale, independent approval, audit |

## 13. Business acceptance criteria

1. A bank can register and govern internal, vendor, predictive, generative, and embedded AI use cases under different jurisdictions and entity policies.
2. An approved case can be reproduced with its questionnaire, ruleset, reviewers, evidence, findings, conditions, exceptions, versions, and decision.
3. A configured material change automatically identifies and reopens the affected obligations.
4. No unauthorized user can discover, view, export, or retrieve restricted use-case/evidence data through UI, API, search, or AI assistance.
5. Monitoring breaches, incidents, complaints, and expiring controls are routed and escalated according to policy.
6. Committee, audit, and regulatory evidence packs can be generated from immutable source records.

## 14. Regulatory references

- [European Commission — AI Act overview and application timeline](https://digital-strategy.ec.europa.eu/en/policies/regulatory-framework-ai)
- [EUR-Lex — Regulation (EU) 2024/1689](https://eur-lex.europa.eu/eli/reg/2024/1689/oj)
- [European Commission — GPAI provider guidelines](https://digital-strategy.ec.europa.eu/en/policies/guidelines-gpai-providers)

These references define a baseline, not legal advice. The implementation must use institution-approved legal interpretations and effective-dated regulatory content.

