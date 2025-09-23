# Selleris – Cooperation Terms (Skeleton / Draft)

Status: Draft (Placeholders)  
Intended Audience: Prospective and current clients  
Language: English (authoritative)  

> NOTE: This is an initial structural draft. Sections marked with TODO will be completed after internal alignment. Do not treat this as the final contractual baseline.

## Table of Contents
- [1. Purpose](#1-purpose)
- [2. Scope of Engagement](#2-scope-of-engagement)
- [3. Roles & Responsibilities](#3-roles--responsibilities)
- [4. Communication & Cadence](#4-communication--cadence)
- [5. Delivery Process](#5-delivery-process)
- [6. Quality & Testing](#6-quality--testing)
- [7. Intellectual Property (IP)](#7-intellectual-property-ip)
- [8. Confidentiality & Data Protection](#8-confidentiality--data-protection)
- [9. Security & Compliance](#9-security--compliance)
- [10. Change Management](#10-change-management)
- [11. Service Levels](#11-service-levels)
- [12. Pricing & Invoicing (Draft)](#12-pricing--invoicing-draft)
- [12A. Estimation & Work Decomposition (Draft)](#12a-estimation--work-decomposition-draft)
- [13. Tools & Environments](#13-tools--environments)
- [14. Dependencies & Assumptions](#14-dependencies--assumptions)
- [15. Risk Management (Draft)](#15-risk-management-draft)
- [16. Termination & Suspension (Placeholder)](#16-termination--suspension-placeholder)
- [17. Dispute Resolution (Placeholder)](#17-dispute-resolution-placeholder)

## 1. Purpose
Outline the standard framework governing commercial collaboration between Selleris and its clients, ensuring clarity on scope, responsibilities, deliverables, communication, ownership, and compliance.

Applicability: These cooperation terms apply automatically to every Selleris client unless superseded or explicitly amended by a separately executed master / project agreement. In the absence of conflicting language, these terms prevail as the operational baseline.

Acceptance: A client is deemed to have accepted these cooperation terms by creating ("posting") a task in the Selleris client portal at `my.selleris.com` or by continuing to use the portal after publication of an updated version. If a client cannot use the portal for technical reasons, a temporary alternative must be mutually confirmed in writing; otherwise the standard acceptance trigger does not change.

Mission Alignment: Deliver measurable, real business value to clients by transforming every approved task into a discrete, reviewable asset (code or documented artifact) within a transparent planning that provides clear roadmaps, committed delivery plans, and traceable outcomes.

## 2. Scope of Engagement
- Engagement Models (Authoritative): Selleris deliberately supports only two commercial delivery models (a) Time & Materials (T&M), (b) Project Stage Model (fixed, pre-approved task set). This constraint preserves transparency, minimizes contractual complexity, and ensures every delivered unit is a discrete, inspectable asset (see Mission Alignment).
- Deliverable Types: Software source code, configuration, integration adapters, scripts, technical/design documentation, advisory analysis, operational improvements, incident mitigation artifacts.
- Out of Scope Examples (unless expressly agreed): Infrastructure hosting / managed cloud operations, software licensing of third-party products, legal or regulatory certification, bespoke penetration testing, end-user training beyond documented handover, data entry / content population.

### 2.1 Time & Materials (T&M) Model
Purpose: Flexible, iterative flow of work where prioritization can shift sprint-to-sprint without renegotiating fixed scope.
Key Characteristics:
- Task-Level Commitment: Each approved task is an independent commercial unit (minimum billable increment rules apply – Section 12).
- Flexibility: High; backlog adjusted via task creation, re-estimation, or cancellation before start.
- Billing Trigger: Hours actually spent on tasks accepted/confirmed within the calendar month (Section 12.4.1).
- Change Handling: Simply shape new or revised tasks; no formal CR unless tied to an approved Stage.
- Risk Allocation: Scope / volume risk primarily on client (they control intake); delivery quality risk on Selleris.
Inclusions: Engineering, code review, lightweight documentation, coordination, small discovery spikes (XS/S).  
Exclusions: Large pre-project discovery (handled as Stage if packaged), guaranteed reserved capacity (unless separately reserved), fixed milestone commitments.

### 2.2 Project Stage Model
Purpose: Predictable delivery of a well-defined feature set or phase where upfront clarity enables coordinated release or investment decisions.
Key Characteristics:
- Stage Definition: Finite, enumerated task list (each task remains discrete) with consolidated estimate and acceptance criteria.
- Billing Trigger: 50% upfront, 50% after all Stage tasks accepted (Section 12.4.2).
- Scope Control: Additions / alterations require a formal Change Request or deferral to a subsequent Stage.
- Flexibility: Lower than T&M during execution; higher predictability of commercial exposure.
- Risk Allocation: Estimate / efficiency risk partially shared—Selleris commits to structured scope; client commits to stable requirements.
Inclusions: Engineering, agreed documentation, handover session(s), internal QA.  
Exclusions: Continuous backlog grooming beyond Stage scope, emergent features not listed at approval.

### 2.3 Model Comparison
| Criterion | T&M | Project Stage |
|----------|-----|---------------|
| Primary Use Case | Ongoing evolution, support, incremental improvements | Cohesive feature release / milestone package |
| Scope Flexibility During Execution | High – tasks can be added/removed anytime pre-start | Low – locked; changes via CR or next Stage |
| Cost Predictability (Per Period) | Variable (driven by approved tasks) | High (pre-approved financial exposure) |
| Start Lead Time | Minimal (task creation & approval) | Moderate (scoping + consolidation + approval) |
| Change Handling | Create/adjust tasks; re-estimate | Formal CR or defer |
| Billing Trigger | Accepted tasks hours in month | 50% upfront / 50% on acceptance |
| Risk of Scope Creep | Managed by task gating | Mitigated by locked Stage boundary |
| Ideal for Uncertainty Level | Higher uncertainty / evolving product | Lower uncertainty / well-understood scope |
| Cancellation Impact | Stop creating/approving tasks | Requires Stage amendment or termination clause |

### 2.4 Selecting a Model
- Choose T&M when discovery continues, priorities may shift, or rapid iteration matters more than fixed financial caps.
- Choose Project Stage when aligning cross-team launches, budgeting for a defined deliverable, or when executive stakeholders need a bounded commitment.
- Combination: A client can run one or more Stages while still submitting T&M tasks for unrelated incremental improvements (governed by Section 12.4.3).

### 2.5 Governance Alignment
Both models enforce the principle of discrete, measurable output per task. No “continuous vague service” classification exists; if sustained capacity is needed, it is still expressed as a series of tasks (T&M) or successive Stages.

No additional engagement forms (e.g., generic retainers or indefinite support subscriptions) are offered unless incorporated as structured Stages or pre-approved T&M task sequences.

## 3. Roles & Responsibilities
The following roles describe functional responsibilities only. Individual names and direct contact details are intentionally excluded in this public document. Some roles may be consolidated depending on engagement scale.

| Role | Primary Focus / Purpose | Selleris Core Responsibilities | Client Collaboration Touchpoints |
|------|-------------------------|--------------------------------|----------------------------------|
| Product Owner (Selleris) | Value alignment & backlog clarity | Refine requirements into discrete tasks; define acceptance criteria; prioritize based on client value & risk; validate delivered increments | Receives business context, negotiates priorities, confirms acceptance readiness |
| Technical Lead | Technical direction & solution integrity | Architecture decisions; code review standards; risk & feasibility assessment; technical debt management; mentoring | Aligns on technical constraints, reviews integration assumptions |
| Delivery Manager | Flow, predictability & coordination | Sprint / iteration orchestration; SLA monitoring; impediment escalation; reporting of progress & risks | Shares roadmap inputs; provides timely approvals / feedback |
| Security / Compliance | Secure development & basic compliance posture | Security review of changes (as scope requires); dependency & vulnerability scanning; guidance on secure configurations; incident triage coordination | Provides required policies, raises security concerns, supplies compliance constraints |
| Support / Success | Post‑delivery continuity & incident responsiveness | Initial triage of incoming tasks; classification & prioritization checks; communication during Critical incidents; organizing knowledge transfer | Supplies reproduction details; validates fixes; provides impact statements |
| DevOps / Platform | Environment reliability & delivery automation | CI/CD pipeline configuration; infrastructure as code (if in scope); observability enablement; performance baseline monitoring; release facilitation | Provides access credentials, environment policies, cost constraints |
| Data Engineer / Analyst (Optional) | Data pipeline & insight enablement | Data model alignment; transformation scripts; data quality checks; basic analytics extracts / dashboards (if in scope) | Supplies source data clarity; confirms metric definitions |
| AI Engineer (Optional) | ML/AI feature integration & lifecycle | Model integration & evaluation harnesses; prompt / inference pipeline optimization; reproducibility & versioning of model artifacts (if ML/AI scope exists) | Defines business success metrics (precision/recall, latency); provides domain feedback on model outputs |

Notes:
- Optional roles are engaged only when the task portfolio justifies their involvement.
- A single individual may fulfill multiple roles in small-scale engagements.
- Escalation Path (draft – to be finalized in Section 11 when escalation matrix is added): Support / Success → Delivery Manager → Technical Lead / Security (depending on nature) → Executive Sponsor (if required).

## 4. Communication & Cadence
- Authoritative Task Channel: All work, questions, change requests, incident reports, and clarifications MUST be created as tasks in the Selleris client portal `my.selleris.com`. This is the single system of record and the sole trigger for SLA timers.
- Emergency Channel (Critical Only): A dedicated Microsoft Teams channel (or chat) may be used strictly for urgent coordination when a Critical priority issue (see Section 11) is actively impacting production or a committed milestone. The Teams channel does not replace the requirement to open / update the portal task; any verbal/chat notice must be followed by a portal task (or reference an existing one) without delay.
- Prohibited Uses of Emergency Channel: Routine status queries, feature ideation, backlog grooming, or non-critical bug triage.
- Cadence (Draft):
	- Weekly or bi‑weekly operational sync (optional where async suffices).
	- Monthly steering / roadmap review (for engagements > 2 months).
- Change Requests: Always logged as a task with type "Change"; impact (cost/time) assessment posted in task before client approval.
- SLA Clock Mechanics: The first‑response SLA timer starts at the timestamp of task creation. It is reset (restarted) upon each new client comment that requires Selleris input. Internal Selleris comments do not reset SLA timers.
- Business Hours (Authoritative): 09:00–18:00 Monday–Friday, Europe/Warsaw timezone (CET/CEST). Tasks created outside Business Hours are timestamped, but SLA hour counting begins at the next Business Hour boundary unless the task is legitimately Critical and notified through the Emergency Channel.
- After-Hours Engagement: Work performed outside Business Hours, on weekends, or on Poland public holidays is billable at double the Base Hourly Rate (see Section 12) unless otherwise contractually agreed. Initiation of after-hours work (except for qualifying Critical incidents) requires explicit written confirmation in the task or the Emergency Channel followed by task documentation.

Holiday Calendar: Polish national public holidays are treated as non-business days unless a separate support addendum states otherwise.

## 5. Delivery Process
1. Initiation: Requirements intake & risk pre‑assessment.  
2. Planning: Backlog shaping, estimation guidelines.  
3. Implementation: Iterative delivery, code review, QA.  
4. Acceptance: Criteria confirmation, UAT support.  
5. Transition: Handover, documentation, knowledge transfer.  

All tasks are managed in GitHub Projects (Projects V2) under an Enterprise license providing granular permission scopes, audit logging, branch protection, and security scanning (Dependabot / code scanning) for traceable, secure lifecycle management.

### 5.1 Minimal Acceptance Criteria Template (Standard)
To keep collaboration lightweight while preserving clarity, each task MUST contain the following minimal structured elements (Variant A – Mandatory Core):

1. Business Outcome: One concise sentence describing the value or change ("Enable X so that Y").  
2. Scope Includes: Bullet list of what is being delivered (functional slice, component, endpoint, UI element).  
3. Out of Scope: Explicit bullets of what is NOT included (prevents assumption creep).  
4. Functional Criteria: List OR simple Given/When/Then statements (at least one); describes observable behavior.  
5. Non-Functional (If Relevant): Only if there is a meaningful performance, security, or UX nuance; otherwise omit.  
6. Acceptance Evidence Required: What the client will review (e.g., PR link, screenshot, test output, curl example).  
7. Data / Migration Impact: "N/A" or note of schema change, migration script, seeded data, backward compatibility note.

Optional Enhancements (used only when warranted by complexity): rollback plan, risk note, edge case enumeration.

### 5.2 Example (Illustrative)
Business Outcome: Allow managers to export quarterly sales summary to CSV for finance reconciliation.

Scope Includes:
- New backend endpoint: GET /reports/sales/quarterly?year=YYYY&quarter=Q
- CSV generation (UTF-8, semicolon delimiter)
- Basic access control (role: manager)

Out of Scope:
- UI dashboard redesign
- XLSX export
- Historical data backfill corrections

Functional Criteria:
- Given a user with role manager, When they request an existing quarter, Then a CSV file is returned (HTTP 200) containing aggregated totals per region.
- Given a user without manager role, When they request the same endpoint, Then HTTP 403 is returned.

Non-Functional (If Relevant): Response time ≤ 2s for datasets ≤ 50k rows.

Acceptance Evidence Required: PR #, automated test report (endpoint tests), sample CSV attached to task.

Data / Migration Impact: N/A (derives from existing sales table; no schema change).

### 5.3 Usage Notes
- If any mandatory element is missing at implementation start, the task may be paused for clarification.
- For XS tasks: Scope Includes may be a single bullet; Non-Functional can be omitted entirely if irrelevant.
- Avoid embedding large discussions in criteria; keep them in comment thread—criteria reflect final agreed snapshot.
- Functional Criteria should focus on externally verifiable outcomes rather than internal implementation details.

### 5.4 Definition of Done (Preview)
The formal Definition of Done matrix will follow (separate subsection) and ties directly to ensuring every Acceptance Criterion is satisfiable, testable, and evidenced. (Will be expanded in a subsequent revision.)

## 6. Quality & Testing
- Code Standards: Internal engineering guidelines (public summary TBD).  
- Testing Levels: Unit, integration, security scanning, performance (on demand).  
- Defect Severity Levels & Remediation Targets defined below.  

### 6.1 Defect Severity Classification
Security findings are mapped directly onto this same severity scale (Option B-1). A security vulnerability that could realistically escalate impact is reclassified upward at Selleris' discretion after client notification.

| Severity | Label | Definition (Impact) | Typical Examples | Workaround Target | Fix / Resolution Target | Notes |
|----------|-------|---------------------|------------------|-------------------|-------------------------|-------|
| S1 | Critical | Production outage, data loss/corruption risk, active security exploit, contractual milestone blocked, no reasonable workaround. | Service down, data integrity failure, privilege escalation vuln, release pipeline blocked for imminent launch. | ≤ 4 hours (stabilize or mitigate) | ≤ 2 business days (or interim mitigation + agreed plan) | Continuous focused effort until stabilized. After-hours engagement may apply. |
| S2 | High | Major functionality broken or severely degraded; costly/risky workaround; security weakness with elevated risk but no active exploit; impacts key user cohort. | Core feature fails for subset, payment flow partial failure, high-severity library vuln w/ no immediate exploit known. | N/A (aim to reduce urgency quickly) | ≤ 5 business days (business hours) | Escalated if risk of becoming S1. |
| S3 | Medium | Partial impairment; acceptable workaround exists; limited user or functional scope; moderate business impact. | Non-critical API returning incorrect secondary field; UI action requires manual retry; moderate performance degradation. | Handled in planned sprint cadence | Next planned release / sprint (typically ≤ 15 business days) | Can be bundled with related fixes. |
| S4 | Low | Minor defect, cosmetic in nature, negligible business impact; does not impede workflows. | Alignment glitch, minor log noise, typo not causing ambiguity. | Not required | Scheduled per prioritization / grouping | May be upgraded if pattern emerges. |
| S5 | Trivial | Purely cosmetic or editorial; no functional impact; polish-only. | Spacing, micro-copy punctuation, color shade mismatch. | Not required | Opportunistic (no guaranteed window) | Can close as "Won't Fix" if superseded by redesign. |

### 6.2 Remediation Principles
- Numeric windows are targets, not guaranteed contractual SLAs unless explicitly added to a support addendum.
- For S1: If full fix cannot meet target, documented mitigation (feature flag isolation, traffic reroute, temporary patch) must be in place while final remedy is scheduled.
- Security: Any S2 security issue demonstrating exploit feasibility or active scanning trend may be escalated to S1.
- Reclassification: Severity may change upon new evidence (impact expansion / mitigation discovery). Changes are logged in task history.
- Evidence of Fix: Must include reference to merged PR, test evidence, and if security-related, a short verification note (e.g. scanner output snippet or manual test).

### 6.3 Tracking & Reporting
- All S1/S2 issues highlighted in weekly (or ad hoc) status summaries until closure.
- Aging S3 (> 2 sprints) triggers review for reprioritization or explicit deprioritize rationale.
- S4/S5 may be grouped into periodic quality batches.

### 6.4 Test Coverage Expectations (Baseline)
- New critical logic (auth, finance-like flows, data transforms): unit + integration test coverage with negative path.
- Public / external API changes: contract test updated; backward compatibility stated.
- Security Fix PRs: regression test or rule (lint/policy) to prevent recurrence where feasible.

### 6.5 Continuous Improvement
Severity distribution and mean time to resolution (MTTR) for S1–S3 are reviewed quarterly to identify systemic issues (e.g., recurring root cause categories).


## 7. Intellectual Property (IP)
This Section allocates ownership and usage rights to balance (a) client certainty over custom business logic and deliverables, with (b) Selleris' need to retain & re‑use internal accelerators, platform capabilities, generic patterns, and know‑how. Code transfer does NOT imply any obligation for Selleris to continue providing hosting, infrastructure, SRE, or managed platform services (see 7.4); those services, when provided, are rendered under a separate hosting / platform agreement and are not governed here.

### 7.1 Definitions
- "Custom Deliverables" – Source code files, configuration manifests, schemas, scripts, technical design documents, migration procedures, and other discrete software or documentation assets created by Selleris specifically for the client under approved tasks / Stages and not constituting Pre‑Existing Materials.
- "Pre‑Existing Materials" – Any tools, libraries, templates, internal frameworks, automation scripts, deployment pipelines, architectural patterns, knowledge bases, runbooks, or other materials owned, developed, or licensed by Selleris (or its licensors) prior to (or independent of) the specific client task, including generic modules refined while serving multiple clients.
- "Composite Work" – A deliverable that intermixes Custom Deliverables with Pre‑Existing Materials.
- "Third‑Party Components" – Open-source or commercially licensed software governed by separate public or vendor licenses.
- "Residual Knowledge" – General ideas, concepts, methods, know‑how, expertise, and skills retained in the unaided memory of Selleris personnel after performing the services.

### 7.2 Ownership of Client-Funded Custom Deliverables
Subject to full payment of all undisputed fees relating to the task(s) producing them, Selleris assigns to the client all right, title, and interest in the Custom Deliverables (excluding Pre‑Existing Materials and Third‑Party Components embedded therein). Assignment is effective upon receipt of payment for the invoice covering the related effort. Until payment, Client holds a revocable, non-transferable right to use the Custom Deliverables solely for internal evaluation.

### 7.3 Selleris Pre-Existing & Retained Materials
All Pre‑Existing Materials remain the exclusive property of Selleris or its licensors. To the extent any Pre‑Existing Materials are incorporated into a Composite Work, Selleris grants the client a perpetual, worldwide, non-exclusive, non-transferable (except with the client’s business successor in an M&A transaction), royalty-free license to use, execute, reproduce and internally modify such embedded Pre‑Existing Materials solely as part of, and to the extent required to utilize, the associated Custom Deliverables. No rights are granted to disassemble generic modules for purposes unrelated to the delivered business functionality or to create derivative products that replicate Selleris’ generic accelerators for redistribution.

### 7.4 Managed Infrastructure & Platform Services (Non-Transfer)
Infrastructure, platform orchestration layers, shared multi-tenant operational tooling, observability stacks, secret management systems, CI/CD pipeline engines, deployment runners, container base images, and any managed runtime configurations that Selleris operates on its own (or third-party) hosting accounts are NOT part of the Custom Deliverables and are not transferred. Access to build or runtime environments while Selleris is the hosting provider is governed by a separate hosting / platform service arrangement. Upon termination or migration, Selleris will (on request) export application-level artifacts (source, build manifests, environment variable names without secret values, configuration templates) – see 7.9.

### 7.5 Open-Source & Third-Party Components
1. All Third‑Party Components are provided under their respective licenses; those licenses govern use, not this Agreement.  
2. Selleris will avoid introducing components with materially restrictive terms (e.g., strong copyleft affecting proprietary aggregation) without advance client notification and written acknowledgment.  
3. A Software Bill of Materials (SBOM) or dependency manifest (e.g., `package.json`, `requirements.txt`, lockfiles) serves as disclosure; additional structured SBOM export may be provided upon request.  
4. Client agrees to comply with attribution, notice, and license retention obligations inherent in such Third‑Party Components.  
5. Security or license compliance obligations beyond reasonable standard dependency hygiene (e.g., formal OSS license audits) require separate scoping.  

### 7.6 License Grants (Assignment & License-Back)
1. Assignment: As per 7.2, Selleris assigns ownership of Custom Deliverables upon full payment.  
2. License-Back to Selleris: Client grants Selleris a perpetual, worldwide, royalty-free, non-exclusive license to internally use (but not publicly distribute as-is) generic patterns, abstractions, or snippets extracted from Custom Deliverables solely for: (a) improving internal tooling, (b) developing reusable accelerators, and (c) knowledge sharing across Selleris teams—provided such reuse does not disclose client Confidential Information or replicate proprietary business logic verbatim.  
3. Analytics / Benchmarking: Selleris may compile and internally use aggregated, anonymized metrics (e.g., build durations, defect density) derived from work performed, excluding client-identifiable data.  

### 7.7 Residuals
Selleris and its personnel are free to use Residual Knowledge for any purpose, including serving other clients, so long as such use does not breach confidentiality or result in unauthorized disclosure of client proprietary source code, trade secrets, or non-public business strategies.

### 7.8 Delivery & Access Mechanics
1. Source Code Delivery: Unless otherwise agreed, source repositories (or mirrored forks) are pushed or granted read access in the client-controlled version control system upon (a) acceptance of the task or (b) periodic sync points for ongoing epics.  
2. Interim Access: If development occurs initially in a Selleris-managed private repository for acceleration reasons, the full commit history (not squashed unless client requests) is provided at delivery checkpoint.  
3. Tooling Scripts: Build scripts, migration scripts, and environment templates (sans secrets) are included within the repository or separate ops folder.  
4. Secrets: Actual secret values (API keys, passwords, tokens) are never stored in code and are not “deliverables”; Selleris supplies the list of required secret names & types.  
5. Binary Artifacts: Container images or compiled binaries built in Selleris infrastructure are reproducible by the client using provided Dockerfiles / build instructions unless a proprietary Selleris base image is involved; in that case a runtime-compatible public base alternative is documented if dependency prohibits redistribution.  

### 7.9 Migration / Exit Assistance
Upon written request within 30 days of termination or transition from Selleris-managed hosting to client-managed infrastructure, Selleris will provide: (a) final source snapshot confirmation, (b) documented environment variable map (names + purpose), (c) infrastructure topology diagram (logical) if previously created under an approved task, (d) data export guidance for application-owned databases (if within scope). Additional hands-on migration support is billable under prevailing T&M rates unless already included in a separately approved Stage.

### 7.10 Warranty & Disclaimer
1. Limited Warranty: For 30 calendar days following acceptance of a Custom Deliverable, Selleris will remediate (at no additional cost) reproducible defects where the implementation materially fails to meet the documented acceptance criteria (Section 5) existing at acceptance date, provided the code has not been modified by the client or third parties in the relevant area.  
2. Exclusions: Issues caused by (a) changes to third-party services outside Selleris control, (b) misuse, (c) environments materially differing from those documented, or (d) unsupported modifications, are out of scope and billable as new tasks.  
3. Disclaimer: EXCEPT FOR THE LIMITED WARRANTY ABOVE, CUSTOM DELIVERABLES AND ANY EMBEDDED PRE‑EXISTING MATERIALS ARE PROVIDED "AS IS" WITHOUT OTHER EXPRESS OR IMPLIED WARRANTIES (INCLUDING MERCHANTABILITY, FITNESS FOR PARTICULAR PURPOSE, NON-INFRINGEMENT).  
4. Mitigation Priority: Warranty fixes are prioritized consistent with severity (Section 6) and do not expand acceptance criteria retroactively.  

### 7.11 Precedence & Survival
In the event of conflict between this Section and any future master agreement, the master agreement prevails. Sections 7.3–7.11 (rights retention, license-back, residuals, disclaimers) survive termination.

## 8. Confidentiality & Data Protection
Selleris treats protection of client confidential information and any personal data as a foundational obligation. This Section summarizes the baseline operational safeguards in place. More stringent, client‑specific controls (if required) can be addressed through a Data Processing Addendum (DPA) or Security Addendum.

### 8.1 Confidential Information
Each party will (a) use the other party’s Confidential Information only for purposes of performing or receiving the services; (b) restrict disclosure to personnel (including vetted subcontractors, if any) with a strict need to know; (c) apply at least the same degree of care it uses to protect its own comparable confidential information (and not less than a commercially reasonable standard). Confidential Information excludes information that is or becomes public without breach, is independently developed, or rightfully obtained from a third party without duty of confidentiality.

### 8.2 Data Minimization & Retention
Selleris collects and stores only the minimum client data required to perform approved tasks. Non-essential production data copies are avoided; where test datasets are required, anonymized or masked samples are preferred. Unless mandated by law or active dispute, transient working data (temporary exports, debug snapshots) are purged within 30 days of resolution of the related task.

### 8.3 Personal Data Handling
If personal data (as defined by applicable data protection laws) is processed, it is limited to the scope necessary for the agreed functionality or debugging. A separate DPA (if executed) will prevail for specifics (data subject rights, international transfers, sub‑processors). In absence of a DPA, Selleris acts as a processor only for the minimal technical purposes inherent to providing development and support services.

### 8.4 Access Control & Identity
- Identity Stack: Microsoft 365 / Azure Active Directory (Entra ID) centralizes identity & conditional access.  
- MFA: Mandatory multi-factor authentication enforced for all privileged and source control accounts.  
- Least Privilege: Access is provisioned per-role and periodically reviewed (at least quarterly) with immediate revocation upon role change or termination.  
- Segregation: Production credentials are isolated; developers operate primarily in non-production environments unless production access is explicitly approved for a task (e.g., incident mitigation).  

### 8.5 Secret & Key Management
All operational secrets (API keys, connection strings, certificates, signing keys) are stored in Azure Key Vault. Direct embedding of secrets in source code, commit history, or unencrypted configuration repositories is prohibited by internal policy and enforced through automated scanning (e.g., GitHub secret scanning and custom pre-commit hooks). Rotation of sensitive keys follows a risk-based schedule or is triggered immediately upon suspected exposure.

### 8.6 Encryption
- In Transit: All external and administrative access endpoints require TLS (minimum TLS 1.2; higher where platform supports).  
- At Rest: Azure-managed disk, database, and object storage encryption (AES-256 or provider equivalent) is relied upon.  
- Backups: Encrypted by the underlying Azure storage subsystem; logical backups containing sensitive data follow the same Key Vault–controlled access restrictions.

### 8.7 Logging & Monitoring
Operational and security-relevant events (authentication, privilege elevation, secret retrieval, deployment actions) are logged in Azure Monitor / Log Analytics and, where applicable, GitHub Enterprise audit logs. Alerting thresholds are configured for anomalous authentication patterns and failed secret retrieval attempts.

### 8.8 Data Transfer & Isolation
Source code and build artifacts are transferred only over encrypted channels (HTTPS / SSH). Where multi-tenant build infrastructure is used, logical isolation and ephemeral build agents minimize persistence of client artifacts beyond build completion.

### 8.9 Confidential Materials Exclusions
Selleris does not accept (and client must not provide) raw production payment card full PAN data, unmasked national IDs, or biometric templates unless a specific addendum with enhanced controls is executed in advance.

### 8.10 Return / Destruction
Upon written request or termination, and subject to Section 7 (IP), Selleris will either return or delete (at client election) remaining client Confidential Information not required for statutory retention—confirming completion in writing (deletion certificates or log references may be provided upon request). Aggregated non-identifying metrics and Residual Knowledge are retained per Sections 7.6–7.7.

## 9. Security & Compliance
This Section summarizes Selleris' secure development and operational posture within the Microsoft 365 + Azure + GitHub Enterprise ecosystem. It is not a substitute for a formal audit report; however, it outlines disciplined baseline practices without expanding Selleris’ liability beyond express contractual terms.

### 9.1 Platform & Ecosystem
- Hosting & Runtime: Azure (regional selection per client task requirements).  
- Identity & Access: Azure AD (Entra ID) with conditional access policies (device compliance / MFA).  
- Source Control & CI/CD: GitHub Enterprise (branch protection, required reviews, Dependabot scanning, secret scanning).  
- Secrets: Azure Key Vault (see 8.5).  
- Productivity & Collaboration: Microsoft 365 (Exchange / Teams) with retention & conditional access policies.

### 9.2 Secure Development Lifecycle (Lightweight)
1. Planning: Security considerations captured in acceptance criteria when relevant (e.g., auth, PII handling).  
2. Implementation: Code review mandatory (at least one qualified reviewer) for non-XS tasks; automated linters and security static analysis (GitHub Advanced Security if licensed) run on pull requests.  
3. Testing: High-risk changes (auth flows, cryptographic handling, data migrations) require explicit negative-path tests.  
4. Pre-Deployment: Dependency vulnerability scan & license check; critical / high severity issues (as defined by advisory sources) evaluated before merge.  
5. Post-Deployment: Runtime monitoring & log anomaly review (Azure Monitor, Application Insights where used).  

### 9.3 Vulnerability Handling Workflow
| Stage | Action | Target (Business Hours) | Output |
|-------|--------|-------------------------|--------|
| Detection | Automated scanner / report or client notice | Immediate logging | Task created / tagged security | 
| Triage | Severity & exploitability assessment | ≤ 1 business day | Severity classification (Section 6) |
| Mitigation (S1/S2) | Workaround / containment | S1 ≤ 4h / S2 ≤ 1 bd | Interim mitigation note |
| Fix Implementation | Code / config remediation | S1 ≤ 2 bd / S2 ≤ 5 bd / S3 next release | PR with reference |
| Verification | Re-scan / manual confirm | ≤ 1 bd after merge | Verification comment |
| Closure | Documentation & metrics update | Same day as verification | Closed task w/ evidence |

Targets above are internal objectives (non-contractual unless a separate support SLA addendum states otherwise) and align with Section 6 remediation principles.

### 9.4 Dependency & Patch Management
- Automated dependency monitoring (Dependabot or Renovate equivalent).  
- High severity advisories: review within 1 business day; if exploitable path confirmed, prioritized per S1/S2 mechanics.  
- Routine upgrades: batched on a scheduled cadence (e.g., bi-weekly) to reduce drift.  
- Deprecated / unsupported dependencies flagged for replacement tasks.

### 9.5 Environment Hardening
- Principle of Least Privilege: Scoped managed identities / service principals with minimal role assignments.  
- Network Controls: Use of Azure security groups / firewall rules to restrict administrative surface; public exposure limited to required endpoints.  
- Isolation: Separation of dev/test/stage/prod subscriptions or resource groups; no direct production database writes from developer local machines.  
- Build Integrity: Signed container images where applicable; ephemeral build agents discard workspace after completion.

### 9.6 Logging, Monitoring & Incident Readiness
- Centralized Log Aggregation: Azure Monitor / Log Analytics + GitHub audit logs.  
- Alerting: Threshold & anomaly alerts (authentication failures, unusual secret retrieval patterns).  
- Incident Classification: Incidents mapped to defect severity (Section 6) for unified response.  
- Post-Incident Review: Blameless summary capturing root cause, mitigation, and prevention tasks.  
- Metrics: Mean Time to Mitigate (MTTM) and Mean Time to Resolve (MTTR) tracked for S1/S2 security issues.

### 9.7 SBOM & Transparency
Dependency manifests (and where supported, CycloneDX / SPDX outputs) can be provided upon request. Baseline SBOM generation occurs at major release checkpoints or monthly (whichever first) for active codebases under maintenance.

### 9.8 Certifications & Framework Alignment
At time of this draft, formal third-party certifications (e.g., ISO 27001, SOC 2) may not be held. Practices are guided by principles consistent with widely adopted frameworks (least privilege, MFA, change control, secure SDLC). Should formal attestation be achieved later, updated references will be inserted without altering ownership terms.

### 9.9 Client Responsibilities
Security is a shared responsibility. Client must: (a) avoid transmitting unnecessary sensitive data into tasks or logs; (b) provision timely approvals for mitigations requiring configuration changes; (c) manage its own identity lifecycle for any client-owned accounts; (d) notify Selleris promptly of suspected credential compromise related to shared systems. Delays in these responsibilities may extend resolution targets proportionally.

### 9.10 Non-Expansion of Liability
Nothing in Sections 8 or 9 creates warranties or indemnities beyond those expressly stated elsewhere. These sections describe operational posture for transparency and collaboration efficiency.

## 10. Change Management
- Change Request (CR) Structure: ID, description, rationale, impact, cost/time delta.  
- Approval Flow: Draft – PO -> Selleris Delivery -> Mutual sign‑off.  
TODO: Add turnaround time guidance.

## 11. Service Levels

### 11.1 Priority Definitions
| Priority | Definition (Operational) | Typical Examples (Non-Exhaustive) | Exclusions / Misuse Guidance |
|----------|--------------------------|-----------------------------------|------------------------------|
| Critical | Production system, key business process, or contractual milestone is blocked or severely degraded with no reasonable workaround; immediate coordinated action required. | Outage of a production integration; data corruption detected; security incident suspected; blocking release pipeline failure hours before a contractual go‑live. | Performance annoyance with workaround; cosmetic issues; feature ideas. |
| High | Significant functional impairment or time‑sensitive deliverable at risk; workaround may exist but is costly or risky; impacts a subset of users or a near‑term milestone. | Major feature partially failing; regression affecting important but not all transactions; blocking dependency clarification needed within current sprint. | Requests without near‑term deadline; backlog grooming. |
| Normal | Standard implementation, enhancement, clarification, or defect that does not materially impair current production operations; reasonable scheduling flexibility. | New feature task; non-blocking refactor; documentation request; moderate UI inconsistency. | Anything urgent or blocking release. |
| Low | Non-urgent optimization, minor cosmetic issue, future improvement, or informational inquiry with no delivery impact. | Spelling/typo; minor layout tweak; low-impact refactor suggestion; deferred analytics request. | Do not use for known upcoming critical deadlines. |

If a task's selected priority does not match these definitions, Selleris may unilaterally reclassify it to preserve operational fairness. Patterned misclassification may lead to temporary moderation of client priority inputs.

### 11.2 First Response SLA (Initial Acknowledgement)
The first response is a substantive acknowledgment (not an automated receipt) indicating: (a) understanding or request for clarification, and (b) next action or ETA for deeper analysis.

| Priority | First Response SLA (Business Hours) | Notes |
|----------|-------------------------------------|-------|
| Critical | 2 hours | Continuous engagement until workaround or stabilization. After-hours requires emergency notification; billed at double rate if outside Business Hours. |
| High | 4 business hours | Same business day acknowledgment. |
| Normal | 8 business hours (1 business day) | May be earlier depending on load. |
| Low | 16 business hours (2 business days) | Batched during backlog review cycles. |

SLA Timing Rules (Business Hours Based):
- Start: Timestamp of task creation in `my.selleris.com`; counting of SLA hours occurs only during defined Business Hours (09:00–18:00 Europe/Warsaw Mon–Fri). Example: A High priority task opened Friday 17:30 with a 4-hour SLA has 0.5 hours counted Friday, remaining 3.5 hours resume Monday 09:00.
- Reset: Each new client comment that requires a Selleris answer restarts the response SLA for that task (previous SLA cycle closes upon Selleris answer or expiration). The restart follows the same Business Hours counting rule.
- Suspension: Waiting on client data / access / clarification stops the SLA timer after Selleris has requested the needed input and labeled the task (label taxonomy TBD). Time between the suspension start and client-provided information is excluded from SLA calculation.
- Aggregation: Multiple issues combined into one Critical ticket may be separated and reprioritized to reflect true impact.
- Misprioritization: Reclassified tasks inherit a fresh SLA window from the reclassification timestamp.

Business Hours Definition: Business Hours exclude weekends and Poland public holidays. Activity outside this window is classified as After-Hours for billing unless covered by a specific extended support agreement.

### 11.3 Future Additions (Placeholders)
- Resolution SLAs (dependent on agreed support tier) – TODO.
- Workaround target times – TODO.
- Escalation matrix & contact rotation – TODO.

Misuse & Reclassification: Selleris will communicate the rationale when downgrading a priority. Repeated emergency channel use for non‑Critical matters may result in limited access or enforced cooling-off practices.

TODO: Add business hours & holiday calendar reference once finalized.

## 12. Pricing & Invoicing (Draft)
- Base Hourly Rate: EUR 60 per hour ("Base Hourly Rate") unless otherwise specified in a separately executed contract or addendum.
- After-Hours / Overtime Rate: 2× Base Hourly Rate (EUR 120/hour) for: (a) any work performed outside Business Hours (Section 4), (b) weekends, and (c) Poland public holidays, except where the parties have agreed to an alternative support retainer or fixed extended coverage.
- Billing Models: Time & Materials (hourly / daily), Fixed Scope milestones, Retainer packages.  
- Invoicing Frequency: TODO (e.g., monthly in arrears for T&M; milestone-based for Fixed Scope).  
- Payment Terms: Defined per model below (Section 12.4).  
- Expenses: Pre‑approved only; pass-through at cost with receipts (draft).  
- Currency: EUR is default; alternative currency requires prior written agreement (FX risk allocation TBD).  
- Rate Changes: Selleris may adjust standard rates with 30 days written notice; locked rates in active SOWs remain until SOW completion or renewal.
- Minimum Billing Increment (Authoritative): 2 hours. Any task estimated at or below 2 hours is billed as 2 hours (XS size) and may be started without additional client approval.

### 12.1 Task Acceptance & Authorization Rules
- Auto-Start Threshold: Tasks estimated ≤ 2 hours (XS) are auto-approved and enter execution queue without separate confirmation.
- Approval Required: Tasks estimated > 2 hours require explicit written client approval (task comment stating approval) prior to commencement.
- Overrun Safeguard: If during execution of an XS task it becomes clear that total effort will exceed 2 hours, Selleris pauses at (or as near as practicable to) the 2-hour mark and posts a revised estimate for approval before proceeding.
- Bundling Prohibition: Related but separable XS tasks must not be aggregated artificially to bypass approval processes.
- Task Project Preparation (Pre-Approval Work): For tasks > 2 hours, an initial "Task Project Draft" may be prepared (see Section 12A.8) to refine scope, acceptance criteria, dependencies, and high-level technical approach. This preparatory effort is capped by default at 10% of the proposed base implementation effort and is billable even if the client declines the full implementation estimate (because a discrete analysis & scoping artifact is delivered). If the client wishes NOT to authorize this preparatory analysis for a specific task, that intent must be stated explicitly before work begins.

### 12.2 Estimation Transparency
- Estimate Format: Each task includes (a) T‑shirt size, (b) indicative hour range (if > XS), (c) key assumptions, and (d) risk factors if material.
- Assumption Drift: Material invalid assumptions trigger re-estimation and renewed approval.

### 12.3 Minimum Billing Increment Rationale
The 2-hour minimum covers: context switching, environment preparation, coordination, code review overhead, and documentation updates even for small changes.

Overtime Authorization: Non-Critical after-hours work requires explicit written authorization in the relevant task prior to commencement; absence of objection to an informational notice does not constitute approval.

Late Payment Handling (Placeholder): Interest, suspension triggers, and reactivation fees to be defined.

TODO: Finalize invoicing schedule, payment term, late fee policy, tax treatment (e.g., VAT applicability).

### 12.4 Payment Models
Clients may freely choose either (or both concurrently) of the following payment models. A task is associated with exactly one model at creation via a required classification field (e.g., label: `T&M` or `Project`).

#### 12.4.1 Time & Materials (T&M) Monthly Model
- Scope: All ad hoc, iterative, or flow-based tasks not bound to a prepaid milestone.
- Recording: Actual engineering & related effort (including review, coordination) logged against each task.
- Invoicing Cycle: Aggregated monthly for all T&M tasks completed (status: Confirmed by client) within the calendar month.
- Invoice Issue: Issued within the first 3 business days of the following month.
- Payment Due Date: Payment due no later than the 15th calendar day of the following month (effectively Net 15 from invoice issuance if issued on day 1).
- Disputed Lines: Client must flag any disputed line item within 7 calendar days of invoice date. Undisputed remainder remains payable by the due date.
- Partial Completions (Rollover Policy): Tasks are expected to be sized to finish within a sprint; however, if a task remains open at month end due primarily to client-side delay (feedback, approvals, access) or external dependency outside Selleris control, then:
	1. Selleris posts a Month-End Rollover Note summarizing the completed functional subset, hours consumed, blockers, and residual scope.
	2. Completed scope is accepted (explicitly or deemed accepted if no blocking feedback within 5 business days where only client feedback is pending).
	3. Logged hours to date are billed in that month's invoice.
	4. Remaining scope is re-estimated and migrated to a NEW continuation task linking back to the original.
	5. Original task is closed with status "Partially Accepted (Rollover)" to preserve auditability.
	6. Repeated rollover of similar categories (>2 consecutive months or >2 occurrences per quarter) triggers a mandatory decomposition & process review.
	Tasks delayed by Selleris internal causes do NOT trigger partial billing; instead they remain in progress and are completed before billing (unless mutually agreed otherwise in writing).

#### 12.4.2 Project (Milestone / Stage) Model
- Use Case: Larger, well-defined feature sets or phases where upfront commitment benefits planning.
- Stage Definition: A Stage groups a fixed set of tasks with clear acceptance criteria and a consolidated estimate (sum of constituent tasks; each still independently tracked).
- Estimation & Approval Flow: (a) Draft stage task list + assumptions; (b) Consolidated hour estimate + risk notes; (c) Client approval (written confirmation in portal); (d) Commercial terms locked for the Stage scope.
- Payment Structure: 50% upfront (invoice issued immediately upon Stage approval, payable before execution begins) and 50% upon acceptance of all Stage tasks (final invoice issued after last task marked Accepted).
- Scope Integrity: Adds / changes after approval form a Change Request either (a) added to a subsequent Stage, or (b) explicitly appended with revised financials (requires mutual written consent).
- Acceptance: Stage considered accepted when every Stage task is in Accepted (or explicitly waived) status. Minor residual non-blocking adjustments may be tracked as new T&M tasks if both parties agree.
- Non-Acceptance: If acceptance is withheld, client must provide a consolidated defect / gap list within 5 business days; unresolved silence after that window may trigger deemed acceptance (optional—TBD if adopted contractually).

#### 12.4.3 Mixed Model Operation
- Coexistence: A client may maintain simultaneous T&M flow for incremental improvements while executing one or more Project Stages in parallel.
- Separation of Tracking: Each task must not switch models mid-life. If a T&M task becomes part of an approved Stage, it is closed (with any completed work billed under T&M) and re-created under the Stage before further effort.
- Reporting: Invoices clearly separate T&M summary (hours × rate) and Project Stage milestone payments.
- Priority Interaction: Model classification does not override SLA priority definitions; Critical issues within a Stage may still be addressed immediately. If a Critical issue is Stage-related, remediation effort counts toward Stage scope unless caused by an out-of-scope change.

#### 12.4.4 Example Classification Labels
| Label | Meaning |
|-------|---------|
| model:tm | Standard monthly T&M task |
| model:project | Task belongs to an approved Stage / milestone |
| stage:<identifier> | Groups tasks under a specific Stage (e.g., stage:alpha-launch) |

#### 12.4.5 Model Selection Guidance
- Choose T&M for exploratory, iterative backlog growth, support, maintenance.
- Choose Project for predictable, contiguous work packages with defined ROI / release goals.
- Use Mixed when a strategic initiative (Project) runs while continuous improvements (T&M) must not stall.

#### 12.4.6 Financial Governance Notes (Draft)
- Upfront Stage payment is non-refundable except where Selleris fails to initiate Stage work within an agreed reasonable start window.
- Material Stage underspend (if actual effort < 80% of estimate) may be converted—subject to mutual agreement—into T&M credit or applied to the next Stage.
- Stage overrun risk must be signaled immediately if forecast effort > 110% of estimate; client options: descoping, CR, or conversion of remainder to T&M.

TODO: Define late payment interest rate & suspension thresholds.

#### 12.4.7 Month-End Rollover Governance (Extended Tasks)
This governance clarifies boundaries around the Partial Completions policy:
- Proper Sizing Principle: Rollover is an exception, not a planning tool; tasks should normally conform to Section 12A sizing.
- Non-Eligible Causes: Overscoping, avoidable internal delays, or lack of proactive decomposition by Selleris.
- Eligible Causes: Awaiting client domain clarification, pending stakeholder approval, delayed test data, external vendor API outage.
- Documentation Requirements: Rollover Note must include (a) link to original task, (b) list of delivered acceptance criteria, (c) list of pending criteria with rationale, (d) hour tally, (e) revised estimate for remainder.
- Transparency Option: Client may request conversion of the remainder into a Stage (Project Model) if predictability is desired.
- Metrics & Continuous Improvement: If rollover rate breaches a jointly agreed KPI threshold, a corrective action plan (CAP) is drafted.

## 12A. Estimation & Work Decomposition (Draft)

### 12A.1 T‑Shirt Size Mapping (Indicative)
| Size | Effort Band (Engineering Hours) | Billing Treatment | Typical Use | Decomposition Guidance |
|------|---------------------------------|-------------------|-------------|------------------------|
| XS | 2h fixed (minimum billable) | Auto-approved, billed as 2h | Minor bug fix, small config, copy tweak, simple query/report | Combine only if logically atomic outcome; else keep separate |
| S | >2h – 8h (up to 1 business day) | Requires approval | Small feature, endpoint, structured refactor, test suite addition | Ensure clear acceptance criteria; avoid scope creep |
| M | >8h – 24h (1–3 days) | Requires approval | Multi-endpoint feature, moderate redesign, integration adapter | Consider slicing by vertical user outcome or integration boundary |
| L | >24h – 40h (3–5 days) | Requires approval | Larger feature set, coordinated refactor + tests | Must fit comfortably inside a single sprint with risk buffer |
| XL | >40h – 64h (5–8 days) | Strongly scrutinized | Epic-sized change nearing sprint span | Mandatory review: try to split into independently deliverable increments |
| XXL | >64h (>8 days) | Not allowed as a single task | Program / multi-epic | Decompose into epics → tasks (≤ L each) |

Notes:
- Effort bands are net engineering effort; review & QA time is included in the estimate.
- A single task should not exceed ~30% of an individual contributor's two-week sprint capacity to preserve flow and enable parallelism.
- XL tasks require an explicit decomposition attempt log (short justification why further split degrades value). XXL must be decomposed—no exceptions.

### 12A.2 Sprint Fit Rule
All tasks must fit inside a standard two-week sprint (10 business days). If not feasible, they are decomposed until each resulting task: (a) provides a testable slice of value, (b) has discrete acceptance criteria, (c) does not create hidden coupling with sibling tasks.

### 12A.3 Recommended Decomposition Strategies
1. Vertical Slicing: Deliver an end-to-end thin functional path (UI → API → persistence) instead of layered horizontal cuts.
2. Risk-First: Isolate the highest technical or integration risk component early to fail fast.
3. Interface Stubs: Create stable interfaces / contracts first; subsequent tasks implement internal logic.
4. Feature Flags: Split enablement (flag scaffolding) from full activation to allow partial, safe merges.
5. Data Migration Separation: Migration scripts / data backfill tracked as distinct tasks from feature logic.
6. Observability as Separate Task: Metrics / logging enhancements can be split if they would block feature delivery.

### 12A.4 Estimation Quality Practices
- Use historical velocity and actuals to calibrate future ranges.
- Record actual effort for M and above to enable continuous improvement.
- Flag High Uncertainty (HU) when assumptions exceed an agreed threshold (e.g., unknown third-party API); plan a spike (time-boxed XS/S) before committing to full estimate.

### 12A.5 Re-Estimation Triggers
- Scope increase or acceptance criteria expansion.
- Architectural pivots or dependency changes.
- External integration instability discovered mid-task.
- Performance or security hardening beyond originally assumed baseline.

### 12A.6 Out-of-Band Changes
If an in-progress task requires material direction change, it is paused and split: original task closed with delivered subset; new tasks capture remaining or altered scope to protect traceability.

### 12A.7 Client Collaboration
Clients are encouraged to challenge over-large tasks; early discussion reduces rework and preserves throughput.
#### Example Decomposition: "Self-Service Password Reset" Feature
Client User Story (raw): "As a user I want to reset my password via email so I can regain access without contacting support."  
Initial Risk / Unknowns: Email deliverability (rate limits), token security, UX copy approval, auditing.

High-Level (Undecomposed) Guess: "~24h" (too coarse — spans UI, backend, security, comms, observability). We decompose to create measurable, testable units:

| Task # | Task Title | Description Focus | Size | Base Dev (E) h | Test 10% h | PM 20% h | Total Indicative h |
|--------|------------|-------------------|------|----------------|-----------|----------|--------------------|
| 1 | Task Project Preparation | Refine acceptance criteria, token expiry policy, email template placeholders, audit events list | XS | 2 (min) | — | — | 2.0 |
| 2 | Password Reset Request Endpoint | POST /auth/password-reset: generate signed token, store hash, send event | S | 4 | 0.4 | 0.8 | 5.2 |
| 3 | Password Reset Token Validation & Completion Endpoint | Validate token (expiry + reuse), set new hash, invalidate token | S | 5 | 0.5 | 1.0 | 6.5 |
| 4 | Email Template + Localization | Markdown/HTML template + EN copy, placeholder for future locales | XS | 2 (min) | — | — | 2.0 |
| 5 | UI: Request Form + Success Screen | Simple form + success state (no auth) | S | 4 | 0.4 | 0.8 | 5.2 |
| 6 | UI: Reset Form + Validation | New password + confirm + strength hints | S | 5 | 0.5 | 1.0 | 6.5 |
| 7 | Security & Abuse Controls | Rate limiting, token TTL config, lockout on brute-force guess patterns | M | 8 | 0.8 | 1.6 | 10.4 |
| 8 | Audit & Logging Events | Emit structured events (request issued, token used, password updated) | XS | 2 (min) | — | — | 2.0 |
| 9 | Integration & Negative Tests | Cross-endpoint flow tests + invalid token, expired token, reused token | S | 4 | (Already partially covered) 0.4 | 0.8 | 5.2 |
| 10 | Observability Dashboards | Basic metrics & alert (excessive resets/hour) | XS | 2 (min) | — | — | 2.0 |
| 11 | Feature Flag Rollout | Wrap UI exposure + endpoints gating (progressive enable) | XS | 2 (min) | — | — | 2.0 |

Notes:
- Preparation effort captured once (Task #1) — not duplicated per task.
- XS tasks use 2h minimum; overhead (test/PM) is considered embedded for XS classification.
- For Tasks 2–7 & 9 (non-XS), Test 10% + PM 20% shown; minor rounding may occur.
- Task #9 (Integration Tests) focuses dedicated testing beyond embedded task-level checks; its own overhead uses the standard percentages.
- If during execution Task #7 expands (e.g., adding CAPTCHA), it may be split into a new S task to maintain granularity.

Roll-Up (Indicative):
- Base Dev Sum (E_total) = 4 + 5 + 2 + 4 + 5 + 8 + 2 + 4 + 2 + 2 = 38h (excluding prep XS tasks where E is already the minimum billing quantum; XS dev hours count toward E_total)
- Preparation (separate, billed) = 2h (capped ≤10% of prospective large feature base estimate; 10% of 38h = 3.8h, so 2h is within cap)
- Testing (approx 10% on non-XS tasks) ≈ 0.4 + 0.5 + 0.4 + 0.5 + 0.8 + 0.4 ≈ 3.0h
- PM (approx 20% on non-XS tasks) ≈ 0.8 + 1.0 + 0.8 + 1.0 + 1.6 + 0.8 ≈ 6.8h
- Total Indicative (rounded) ≈ 38 + 2 + 3.0 + 6.8 = 49.8h → 50h (planning number)

Client Review Benefits:
- Each task independently testable & shippable (vertical slices).
- Parallelization possible (e.g., UI tasks vs security controls) to reduce lead time.
- Clear visibility into which parts can be descoped if deadline pressure emerges (e.g., Observability dashboards could move to later sprint without jeopardizing core capability).

Change Handling:
- If UI strength hints require external API after start → create spike XS task; adjust impacted UI task size if needed.
- If legal mandates extended audit fields mid-flight → split new S task rather than inflating existing ones silently.

Outcome: The client can approve granular scope with transparent overhead rationale instead of a single opaque 24–50h block.

### 12A.8 Estimation Workflow & Cost Composition
This subsection clarifies how Selleris structures task estimation and communicates cost components to maintain transparency.

#### 12A.8.1 Stages of a Task
1. Task Project Preparation (Scoping Draft)
	- Input: Client user story / raw requirement.
	- Output: Refined task using minimal acceptance criteria (Section 5.1), clarified assumptions, preliminary sizing.
	- Effort Basis: Up to 10% of base implementation estimate ("Base Dev Effort" E). Billed regardless of later implementation approval because it produces a discrete, reviewable artifact (scope spec / refined acceptance criteria / risk notes).  
2. Implementation
	- Core engineering & code creation aligned to acceptance criteria.
	- Effort Estimate: Base Dev Effort (E) hours.
3. Testing
	- Additional structured test design & execution beyond what is naturally embedded in implementation (e.g. explicit integration scenarios, negative paths, regression verification).  
	- Standard Allocation: 10% of E (T = 0.10E). Adjusted upward only if explicitly stated (e.g. complex data migrations, multi-environment matrix).  
4. Project Management (Lifecycle Oversight)
	- Planning, coordination, stakeholder updates, progress reporting, task state hygiene in GitHub Projects, scheduling of code reviews, risk tracking.
	- Standard Allocation: 20% of E (PM = 0.20E).  

#### 12A.8.2 Formula Summary
Base Dev Effort (E)  
Preparation (Prep) = 0.10E  
Testing (Test) = 0.10E  
Project Management (PM) = 0.20E  
Total Indicative Effort = E + 0.10E + 0.10E + 0.20E = 1.40E

Example: If E = 10h → Total = 14h (Prep 1h, Implementation 10h, Testing 1h, PM 2h).  

#### 12A.8.3 XS Tasks (≤ 2h)
- The 2-hour minimum billing quantum already encompasses preparation, implementation, testing, and PM overhead for genuinely small changes.
- If overhead alone would exceed the minimum (rare edge case), the task should be reclassified and re-estimated as S.

#### 12A.8.4 Transparency in Estimates
Estimates for tasks larger than XS include a breakdown line showing:  
"Base Dev: E h | Prep 10%: 0.10E | Test 10%: 0.10E | PM 20%: 0.20E | Total: 1.40E h".

If any component deviates from defaults (e.g. Testing 25% due to complex data validation), the deviation and reason must be explicitly noted.

#### 12A.8.5 Declined Implementation Scenarios
If the client declines to proceed with implementation after the Task Project Preparation stage:
- Only the Preparation component (actual time, capped at 10% of proposed E) is billed.
- The scoping artifact remains accessible to the client and may be reused in a future task or Stage.

#### 12A.8.6 Re-Estimation Impact
When task scope changes enough to trigger re-estimation (Section 12A.5), percentage components are recalculated against the new Base Dev Effort. Previously incurred preparation remains billed; no retroactive adjustment is made.

#### 12A.8.7 Portfolio View
Over time, Selleris may publish aggregate metrics (e.g. average actual vs estimated prep %, test %, PM %) to improve forecasting accuracy. Clients can request these metrics during quarterly reviews.

#### 12A.8.8 Rationale for Overhead Percentages
- Preparation 10%: Ensures sufficient discovery to avoid rework while keeping friction low.
- Testing 10%: Baseline reinforcement of quality; incentivizes thin vertical slicing which naturally limits test surface area.
- PM 20%: Covers coordination overhead for asynchronous communication, status curation, backlog hygiene, and risk surfacing—especially important in multi-task concurrent flows.

Percentages are baselines, not hard caps in abnormal complexity contexts (e.g. regulated environments); any variance requires explicit pre-approval.

## 13. Tools & Environments
- Source Control: Git-based (platform TBD if externally visible).  
- Tracking: Issue/project management platform (TBD).  
- Knowledge Base: This repository (public subset) + private internal docs.  
TODO: Add access provisioning workflow.

## 14. Dependencies & Assumptions
| Assumption | Rationale | Risk if False | Mitigation (Draft) |
|------------|-----------|--------------|--------------------|
| Timely stakeholder feedback | Maintains iteration velocity | Delays & rework | Escalation path |
| Stable scope within iteration | Protects sprint commitments | Velocity disruption | CR process |
| Access to required test data | Enables validation | Blocked releases | Provide sanitized dataset |

TODO: Add more operational assumptions.

## 15. Risk Management (Draft)
- Identification: During planning and retrospectives.  
- Tracking: Risk register (private).  
- Categories: Delivery, Technical, Compliance, Security.  
TODO: Add risk severity matrix.

## 16. Termination & Suspension (Placeholder)
- Termination Rights: TBD (e.g., notice period, material breach).  
- Suspension Conditions: Non-payment, security concern (draft).  
TODO: Add data return / transition assistance language.

## 17. Dispute Resolution (Placeholder)
Draft: Good faith negotiation -> escalation -> mediation/arbitration (jurisdiction TBD).  
TODO: Define preferred governing law / venue.

---
Feedback: Please consolidate suggested edits and submit internally before publishing externally.
