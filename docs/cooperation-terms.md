# Selleris – Cooperation Terms (Skeleton / Draft)

Status: Draft (Placeholders)  
Intended Audience: Prospective and current clients  
Language: English (authoritative)  

> NOTE: This is an initial structural draft. Sections marked with TODO will be completed after internal alignment. Do not treat this as the final contractual baseline.

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
| Role | Selleris Responsibilities (Draft) | Client Responsibilities (Draft) |
|------|-----------------------------------|---------------------------------|
| Product Owner | TODO | TODO |
| Technical Lead | TODO | TODO |
| Delivery Manager | TODO | TODO |
| Security / Compliance | TODO | TODO |
| Support / Success | TODO | TODO |

TODO: Add escalation contacts / response time placeholders.

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
TODO: Add acceptance criteria template & definition of done matrix.

## 6. Quality & Testing
- Code Standards: Internal engineering guidelines (public summary TBD).  
- Testing Levels: Unit, integration, security scanning, performance (on demand).  
- Defect Severity Levels: TODO (table pending).  
- Remediation Targets: TODO.  

## 7. Intellectual Property (IP)
Draft Principle: Custom deliverables funded by the client become the client's property upon full payment, excluding pre‑existing Selleris frameworks, tools, or accelerators (licensed for use).  
TODO: Refine license boundary wording & include open-source component obligations.

## 8. Confidentiality & Data Protection
- Mutual confidentiality obligations (draft).  
- Data Handling: Minimal retention principle.  
- Personal Data: Processed only as required; DPA addendum if needed.  
TODO: Add encryption & access control summary.  

## 9. Security & Compliance
- Baseline Practices: Version control, MFA, least privilege.  
- Vulnerability Handling: Report & patch workflow (TODO).  
- Third‑Party Dependencies: SBOM transparency (draft).  
TODO: Add certifications / attestations (if any).

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

TODO: Add example decomposition of a hypothetical large feature.

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

## 18. Revision & Versioning
- Each change logged below with date, summary, author.  
- Major vs Minor version criteria (TODO).  

### Revision History
| Version | Date | Author | Summary |
|---------|------|--------|---------|
| 0.1.0-draft | 2025-09-23 | Selleris Docs | Initial structural skeleton |
| 0.2.0-draft | 2025-09-23 | Selleris Docs | Added applicability, acceptance mechanics, communication channels, SLA first response rules & priority definitions |
| 0.3.0-draft | 2025-09-23 | Selleris Docs | Added business hours (Europe/Warsaw), SLA business-hours counting clarification, base & after-hours rates, pricing section expansion |
| 0.4.0-draft | 2025-09-23 | Selleris Docs | Added minimum billing increment, auto-start rule, estimation & t-shirt sizing, decomposition best practices |
| 0.5.0-draft | 2025-09-23 | Selleris Docs | Added payment models (T&M monthly, Project 50/50), mixed model rules, financial governance |
| 0.6.0-draft | 2025-09-23 | Selleris Docs | Added T&M month-end rollover policy & governance for extended tasks |
| 0.7.0-draft | 2025-09-23 | Selleris Docs | Finalized mission alignment statement |

## 19. Glossary (Draft)
| Term | Definition (Placeholder) |
|------|--------------------------|
| DOR | TODO |
| DOD | TODO |
| SLA | TODO |
| CR | TODO |

## 20. Appendix (Future)
- Acceptance Criteria Template (TBD)  
- Definition of Done Matrix (TBD)  
- Severity & Priority Guidelines (TBD)  

---
Feedback: Please consolidate suggested edits and submit internally before publishing externally.
