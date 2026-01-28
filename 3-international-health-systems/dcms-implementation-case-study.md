# Digital Centre Management System (DCMS) Implementation
## A Case Study in Constraint-Driven Healthcare Innovation

### Context & Problem

Between 2021 and 2022, I served as Change Officer for the Digital Centre Management System (DCMS) rollout across 40+ physical rehabilitation centres (PRCs) in conflict-affected regions supported by the International Committee of the Red Cross (ICRC). This experience crystallised a central conviction that now shapes my PhD research focus: healthcare innovation succeeds only when it truly understands the people it is intended for.

#### The Challenge

The ICRC-supported rehabilitation centres faced multiple, interconnected problems:

**Clinical & Data Management:**
- Outdated Patient Management System (PMS) that was no longer sustainable
- Data collected retrospectively in "silo mode"—clinicians entered information days later, disconnected from patient care
- Poor monitoring and reporting due to fastidious paperwork, creating an unclear picture of overall impact
- System was not maintainable by centres once ICRC handed over support

**Operational & Resource Management:**
- Poor stock management at centre level, with items disappearing or being inefficiently used
- Delays in data collection from partner centres due to time-consuming paperwork
- Unclear accountability at each level
- Non-integrated solutions for managing resources (supplies, manufacturing, human resources, dormitory occupancy)

These constraints were not merely technical—they were embedded in the operational realities of conflict-affected settings: limited connectivity, staff capacity constraints, resource scarcity, and the need for systems that local partners could maintain independently.

---

### Solution Architecture

The DCMS was designed as a comprehensive, **open-source digital platform** combining two tools:

**Electronic Medical Record (EMR)** — OpenMRS
- Digitalised clinical data collection at point of care
- Support for multidisciplinary evaluation and care planning
- Appointment management and service tracking
- Referral processes and outreach service documentation
- Automatic population of reporting dashboards (via DHIS2 integration)

**Enterprise Resource Planning (ERP)** — Odoo
- Stock and supply chain management (procurement, forecasting)
- Manufacturing and quality assurance tracking
- Human resources and payroll management
- Financial tracking and service invoicing
- Maintenance scheduling and equipment replacement
- Dormitory occupancy management

#### Modular, Constraint-Responsive Deployment

Critically, the system was designed with **modularity** to adapt to real-world constraints:

| Deployment Size | Clinical Features | Administrative Features | Hardware |
|---|---|---|---|
| **Small** | Retroactive data entry | Stock management | 3 desktops, 1 laptop |
| **Medium** | Point-of-care data entry | Stock + Supply chain + Manufacturing + HR | 6-7 desktops, 6 laptops, 1 tablet per 2 clinicians |
| **Large** | Full point-of-care + outreach | Full ERP (+ Maintenance, Invoicing, Asset management) | 10 desktops, 6 laptops, 1 tablet per clinician |

This modularity respected a fundamental principle: **centres were not forced into standardised solutions that exceeded their capacity or constraints.** Instead, the system scaled with their readiness.

---

### Implementation Approach: Change as a Human Problem

The DCMS deployment was not primarily a technical rollout—it was an **organisational and human transformation** across 80+ centres in multiple countries (Asia, Africa, Middle East). This required systematic change management grounded in understanding behaviour, not just technology adoption.

#### The ADKAR® Change Management Framework

We applied the **ADKAR model** to address the human side of change, recognising that without behaviour change, technology deployment fails:

| ADKAR Level | Focus | Key Challenge | Our Mitigation |
|---|---|---|---|
| **Awareness** | Understanding why change is needed | Centres saw PMS as "working enough" | Clear communication of pain points: inefficiency, unsustainability, lack of data quality |
| **Desire** | Building motivation for change | Potential role abdication among ICRC PRP managers | Training PRP managers on change management; clarity on new support/coaching roles |
| **Knowledge** | Building capability | Staff unfamiliar with digital tools | Cascading training-of-trainers model; role-specific instruction |
| **Ability** | Converting knowledge into practice | Moving from theory to sustainable new workflows | Ongoing support, coaching, feedback loops |
| **Reinforcement** | Sustaining change | Regression to old ways | Quality assurance processes; monitoring dashboards; incentive alignment |

#### Anticipated Resistance & Mitigation

We identified potential blocking points and designed specific interventions:

**Resistance Point: ICRC PRP Managers**
- *Risk:* Role abdication—managers unsure of their position in supporting change
- *Mitigation:* Explicit role redefinition; training in change management principles; clarity that their role shifted from "systems administrator" to "change champion and coach"

**Resistance Point: Partner Centre Staff**
- *Risk:* Insufficient incentives to improve efficiency; reluctance due to low motivation
- *Mitigation:* Advocacy to increase commitment; connecting efficiency gains to centre sustainability and quality improvements for service users

**Resistance Point: Sustainability**
- *Risk:* System viewed as an ICRC imposition; centres unable to maintain it post-handover
- *Mitigation:* Open-source architecture ensuring independence; modular design adapted to centre capacity; focal point training ensuring local expertise

---

### Implementation Structure: Training as Cascading Behaviour Change

The rollout was structured as a **cascading training-of-trainers model**, recognising that sustainable change requires local champions, not external experts.

#### Training Architecture

**Phase 1: Regional Training of Trainers (ToT)**
- Hosted in referral centres (e.g., Kampong Speu, Cambodia; Muzaffarabad, Pakistan)
- Trained a mix of staff: clinical staff (PT/P&O leaders), administrative staff (storekeeper, admin), IT focal points
- Created both EMR and ERP focal points at each centre
- Duration: 6+ months of preparation, cascading globally

**Phase 2: Training of Users (ToU) in Partner Centres**
- Local trainers (who attended ToT) trained their own centre staff
- Role-specific training: clinicians received different instruction than administrative staff
- Timed support structure: intensive support pre-go-live, ongoing support post-go-live

**Phase 3: Ongoing Support Model**
- Dedicated ICT focal point at each centre for technical troubleshooting
- Monthly refresh trainings and Q&A sessions
- Incident reporting and feedback loops for continuous improvement
- PRP managers shifted to a coaching role rather than administrative role

---

### Outcomes & Success Metrics: Beyond Technology Adoption

Critically, we rejected the conventional metric of success: *"How many users adopted the system?"*

Instead, we designed an outcomes framework that measured **clinically meaningful and operationally meaningful change**:

#### Strategic Objectives (ICRC Level)
- Building sustainable humanitarian impact with people affected
- Working with partners to enhance impact
- Embracing digital transformation

#### Benefits Realisation Framework

| Stakeholder | Clinical Benefit | Operational Benefit | Sustainability Outcome |
|---|---|---|---|
| **Service Users** | Reduced wait times; better follow-up and continuity of care; higher quality care | Faster device delivery; improved service flow; better referral processes | N/A |
| **PRC Staff** | Centralised, secure medical records; support for multidisciplinary work; reduced paperwork | Clearer accountability; management dashboard for activity overview; time savings | Capacity to maintain system independently |
| **PRC Management** | Better data for quality improvement | Efficiency improvements (target: 15% staff efficiency ratio improvement); reduced fraud risk; better resource tracking | Sustainable tool (open-source) that can be maintained post-ICRC |
| **ICRC/Partners** | High-granularity clinical data for reporting | Automated data flow (EMR to DHIS2); improved monitoring of overall impact | Data-driven decision-making; new funding mechanisms enabled |

#### Key Performance Indicators

**Efficiency:**
- Staff Efficiency Ratio: Target 15% improvement in resource-to-service-user ratio
- Service flow: Reduced time from assessment to device delivery
- Procurement: Reduced stock shortages and waste

**Quality:**
- Service user satisfaction
- Data quality and completeness
- Multidisciplinary coordination metrics (% of users receiving services across multiple disciplines)

**Sustainability:**
- Number of centres maintaining system independently at hand-over
- Local staff capability to troubleshoot and adapt system
- Centre autonomy in reporting and decision-making

---

### What This Taught Me: Why Neurocognitive Decision-Making Matters

This experience—implementing a digital system across dozens of centres in resource-constrained, conflict-affected settings—taught me something fundamental: **technology succeeds or fails based on human behaviour, not technical elegance.**

The real questions were never about whether OpenMRS or Odoo was technically superior. They were:

- **How does organisational context shape individual behaviour?** A clinician's willingness to enter data at point-of-care depended not just on system usability, but on whether they understood *why* (purpose), *what benefit it brought them* (personally and for patients), and *whether they had time and support* (resources).
- **What motivates sustained behaviour change?** It wasn't compliance; it was agency. Centres that felt ownership of the system—that they shaped it through focal points and feedback—sustained the change.

---

### Key Learnings & Implications

**1. Constraint-Driven Design Works**
Systems designed *with* real-world constraints, not against them, are more sustainable and usable. The modular DCMS succeeded where a "one-size-fits-all" system would have failed.

**2. Human Behaviour ≠ System Adoption**
Technology adoption metrics (user login frequency, form completion rate) tell you nothing about whether the system improved care or outcomes. We needed to measure what clinicians and administrators *actually valued*: time saved, quality improved, autonomy increased.

**3. Change Management is Cognitive & Organisational**
The ADKAR framework worked because it addressed not just individual knowledge and ability, but desire, awareness, and institutional reinforcement. Change is not a technical process; it's a human process embedded in organisational systems.

**4. Behaviour Change Requires Agency**
Centres that felt ownership—where staff participated in training design, where local focal points had authority, where feedback loops shaped the system iteratively—sustained change. Centres where the system was imposed, where external experts "knew best," regressed.

**5. Open-Source Architecture Enables Independence**
The choice of open-source tools (OpenMRS, Odoo) was not just about cost. It was about sustainability and dignity. Partner centres could maintain the system, adapt it, own it. This is fundamentally different from proprietary systems that create dependency.

---

### Conclusion

The DCMS implementation across 80+ physical rehabilitation centres demonstrates a central principle: **healthcare innovation succeeds when it is grounded in real-world constraints, co-designed with end-users, and evaluated on clinically meaningful outcomes—not technology metrics.**

This experience shaped my conviction that to design better healthcare systems, we must understand not just *how* humans use technology, but *why* they make the decisions they do—how they process information under uncertainty, how they adapt to change, how their neurocognitive processes interact with organisational and social context.


---

## References & Artefacts

Some of my own material created for the project:
- DCMS Three-Pager Overview (ICRC, 2021)
- DCMS Master Presentation (Architecture & Modular Deployment)
- DCMS Benefits Mapping Framework (September 2021)
- Change Management for Trainers (ADKAR Model & Stakeholder Analysis)
- Training Architecture & Cascade Structure

*Case study written January 2026, reflecting on 2021-2022 implementation period.*
