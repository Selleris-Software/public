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
- Working Hours Placeholder: Business hours / regional coverage to be defined (see Section 11 notes).

TODO: Add finalized business hours & holiday calendar reference.

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
| Critical | 2 hours | Continuous engagement until workaround or stabilization. Outside standard coverage may require enhanced support addendum. |
| High | 4 business hours | Same business day acknowledgment. |
| Normal | 8 business hours (1 business day) | May be earlier depending on load. |
| Low | 16 business hours (2 business days) | Batched during backlog review cycles. |

SLA Timing Rules:
- Start: Timestamp of task creation in `my.selleris.com`.
- Reset: Each new client comment that requires a Selleris answer restarts the response SLA for that task (previous SLA cycle closes upon Selleris answer or expiration).
- Suspension: Waiting on client data / access / clarification stops the SLA timer after Selleris has requested the needed input and labeled the task (label taxonomy TBD).
- Aggregation: Multiple issues combined into one Critical ticket may be split and reprioritized.

Business Hours Placeholder: Standard coverage window & regional holidays will be specified (still TBD). Until defined, times are interpreted relative to the primary contracted service region.

### 11.3 Future Additions (Placeholders)
- Resolution SLAs (dependent on agreed support tier) – TODO.
- Workaround target times – TODO.
- Escalation matrix & contact rotation – TODO.

Misuse & Reclassification: Selleris will communicate the rationale when downgrading a priority. Repeated emergency channel use for non‑Critical matters may result in limited access or enforced cooling-off practices.

TODO: Add business hours & holiday calendar reference once finalized.

## 12. Pricing & Invoicing (Placeholder)
- Billing Models: Time & Materials (hourly / daily), Fixed Scope milestones, Retainer packages.  
- Invoicing Frequency: TODO.  
- Payment Terms: TODO (e.g., Net 15 / Net 30).  
- Expenses: Pre‑approved only (draft).  
TODO: Add late payment handling & currency policy.

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
