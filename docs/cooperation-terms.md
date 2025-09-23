# Selleris – Cooperation Terms (Skeleton / Draft)

Status: Draft (Placeholders)  
Intended Audience: Prospective and current clients  
Language: English (authoritative)  

> NOTE: This is an initial structural draft. Sections marked with TODO will be completed after internal alignment. Do not treat this as the final contractual baseline.

## 1. Purpose
Outline the standard framework governing commercial collaboration between Selleris and its clients, ensuring clarity on scope, responsibilities, deliverables, communication, ownership, and compliance.

Applicability: These cooperation terms apply automatically to every Selleris client unless superseded or explicitly amended by a separately executed master / project agreement. In the absence of conflicting language, these terms prevail as the operational baseline.

Acceptance: A client is deemed to have accepted these cooperation terms by creating ("posting") a task in the Selleris client portal at `my.selleris.com` or by continuing to use the portal after publication of an updated version. If a client cannot use the portal for technical reasons, a temporary alternative must be mutually confirmed in writing; otherwise the standard acceptance trigger does not change.

Mission Alignment (Draft): Enable predictable, transparent, and secure delivery of value while minimizing friction in communication and prioritization. (Will be refined.)

## 2. Scope of Engagement
- Engagement Models: (e.g., Fixed Scope / Time & Materials / Retainer) – TODO details.
- Deliverable Types: Software components, integrations, advisory, support.  
- Out of Scope Examples: Infrastructure hosting (unless agreed), third‑party licensing, legal compliance certification.  
TODO: Add model comparison table.

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
- Payment Terms: TODO (e.g., Net 15 / Net 30) from invoice date.  
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
| 0.3.0-draft | 2025-09-23 | Selleris Docs | Added business hours (Europe/Warsaw), SLA business-hours counting clarification, base & after-hours rates, pricing section expansion |

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
