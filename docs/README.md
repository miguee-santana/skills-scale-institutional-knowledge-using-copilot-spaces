# OctoAcme Project Management Documentation

## Purpose
This documentation centralizes the OctoAcme project management processes, providing a single source of truth for how we run projects, manage risks, and deliver value.

## Quick Navigation

### Project Lifecycle Stages
- **Initiation**: [OctoAcme Project Initiation Guide](./octoacme-project-initiation.md) - Validate and authorize work, align stakeholders
- **Planning**: [OctoAcme Project Planning](./octoacme-project-planning.md) - Break work into shippable increments
- **Execution & Tracking**: [OctoAcme Execution & Tracking](./octoacme-execution-and-tracking.md) - Manage day-to-day execution
- **Release & Deployment**: [OctoAcme Release & Deployment Guide](./octoacme-release-and-deployment.md) - Standardize releases to production
- **Retrospective & Improvement**: [OctoAcme Retrospective & Continuous Improvement](./octoacme-retrospective-and-continuous-improvement.md) - Capture learnings

### Cross-Cutting Concerns
- **Risk & Communication**: [OctoAcme Risk Management & Communication](./octoacme-risks-and-communication.md) - Manage risks and stakeholder communications
- **Roles & Personas**: [OctoAcme Personas](./octoacme-roles-and-personas.md) - Understand team roles and responsibilities

### Overview
- **Project Management Overview**: [OctoAcme Project Management Overview](./octoacme-project-management-overview.md) - High-level introduction to our approach

## OctoAcme Project Management Approach – Summary

### Project Lifecycle & Workflows
OctoAcme follows a structured, five-phase project lifecycle designed to deliver value iteratively while maintaining clear stakeholder alignment. Projects begin with **Initiation**, where business needs are validated through a lightweight Project One-pager that captures the problem statement, success metrics, and stakeholder requirements. Once approved, teams move into **Planning**, where work is broken into shippable increments, acceptance criteria are defined, and dependencies are mapped. The core **Execution** phase leverages agile practices with daily standups, weekly delivery syncs, and a structured pull request workflow emphasizing small, reviewable changes (≤400 lines). Quality gates include unit tests, integration tests, and security scanning in CI before code merges. After delivery, teams conduct **Release & Deployment** using standardized checklists and smoke tests to minimize production risk, followed by **Retrospectives** to capture learnings and drive continuous improvement.

### Core Roles & Clear Ownership
OctoAcme operates with well-defined personas to ensure accountability and clarity. **Project Managers** coordinate schedules, manage risks, and facilitate communication across stakeholders, maintaining the project timeline and escalation paths. **Product Managers** own the vision, define success metrics, and prioritize the backlog based on customer value and data-driven insights. **Developers** implement features, collaborate on design, and contribute to planning and risk identification. **QA/Testing teams** validate acceptance criteria and quality standards. This clear role separation, combined with the principle that each project has a named PM and Product Lead, eliminates ambiguity and ensures consistent execution across initiatives.

### Communication & Risk Management
Transparency and structured communication are central to OctoAcme's approach. Teams maintain a consistent cadence: daily standups (15 min), weekly PM–Product Lead alignment, twice-weekly delivery team standups, and monthly stakeholder updates. Risk management is formalized through a Risk Register tracking ID, description, impact, likelihood, owner, and mitigation plans—reviewed weekly and escalated through three levels when needed (team-level → PM → Product Lead → Sponsor). Status communication follows a standard template covering progress, next steps, risks, and decisions needed. For incidents, a blameless retrospective approach is used to convert failures into learning opportunities rather than blame.

### Quality & Continuous Improvement
Quality is embedded throughout execution rather than treated as a final step. All work must meet a documented **Definition of Done** before being considered complete, and acceptance criteria are defined during planning to ensure shared understanding. The team tracks velocity, burndown, and success metrics identified in the Project One-pager, using dashboards for key signals like errors, latency, and usage. Retrospectives are held after each sprint or milestone to identify what went well and what can improve, with 2–3 prioritized action items fed back into the project backlog. This cycle of measurement, reflection, and iteration—grounded in psychological safety and customer-first principles—creates a culture of continuous improvement and accountability.

## Core Principles
- **Customer-first**: Prioritize customer value and usability
- **Iterative delivery**: Deliver small, testable increments
- **Clear ownership**: Each project has a named PM and Product Lead
- **Data-informed decisions**: Measure impact and iterate based on evidence
- **Psychological safety**: Encourage feedback and learning

## Key Artifacts & Communication
- **Project Charter / One-pager**: Defines problem, goals, success metrics, stakeholders, timeline
- **Roadmap & Release Plan**: Long-term vision and delivery schedule
- **Sprint/Iteration Backlog**: Prioritized work with acceptance criteria
- **Definition of Done**: Quality standards and checklist for completion
- **Risk Register**: Tracked risks with mitigation plans and owners
- **Retrospective notes**: Learnings and action items for continuous improvement

### Communication Cadence
- Weekly sync between PM and Product Manager
- Twice-weekly standups for delivery team
- Monthly stakeholder updates
- Ad-hoc escalations as needed

## For Your Role

### Developers
Start with these documents to understand your responsibilities and workflows:
- [Execution & Tracking](./octoacme-execution-and-tracking.md) – Day-to-day workflows, PR standards, quality & testing practices
- [Roles & Personas](./octoacme-roles-and-personas.md) – Your responsibilities and how you fit into the project lifecycle
- [Project Planning](./octoacme-project-planning.md) – Definition of Done, acceptance criteria, and backlog structure
- [Risk & Communication](./octoacme-risks-and-communication.md) – Identifying and escalating technical risks

### Product Managers
Start with these documents to manage prioritization, roadmaps, and stakeholder alignment:
- [Project Initiation](./octoacme-project-initiation.md) – Problem statements, success metrics, and go/no-go decisions
- [Project Planning](./octoacme-project-planning.md) – Backlog prioritization, roadmap creation, and acceptance criteria
- [Roles & Personas](./octoacme-roles-and-personas.md) – Your responsibilities and how you work with the delivery team
- [Risk & Communication](./octoacme-risks-and-communication.md) – Stakeholder updates and communication strategies
- [Retrospectives](./octoacme-retrospective-and-continuous-improvement.md) – Capturing learnings and measuring action items

### Project Managers
Review all documents with emphasis on planning, execution, and escalation:
- [Project Initiation](./octoacme-project-initiation.md) – Initiation checklist and decision gates
- [Project Planning](./octoacme-project-planning.md) – Schedule, timeline, and milestone management
- [Execution & Tracking](./octoacme-execution-and-tracking.md) – Daily standup facilitation and status reporting
- [Risk & Communication](./octoacme-risks-and-communication.md) – Risk registers, escalation paths, and stakeholder communication
- [Release & Deployment](./octoacme-release-and-deployment.md) – Release coordination and deployment checklists
- [Retrospectives](./octoacme-retrospective-and-continuous-improvement.md) – Retrospective facilitation and action item tracking

### QA / Testing Teams
Start with:
- [Execution & Tracking](./octoacme-execution-and-tracking.md) – Quality standards, testing practices, and acceptance criteria validation
- [Project Planning](./octoacme-project-planning.md) – Understanding the Definition of Done
- [Release & Deployment](./octoacme-release-and-deployment.md) – Smoke testing and post-deploy verification

## Getting Started

1. **First time here?** Read the [Project Management Overview](./octoacme-project-management-overview.md) for a high-level introduction to OctoAcme's approach.

2. **Find your role** in the "For Your Role" section above and review the recommended documents.

3. **Navigate by project stage** using the Project Lifecycle Stages links above to find guidance for each phase of your project.

4. **Refer to cross-cutting concerns** at any stage:
   - Use [Risk & Communication](./octoacme-risks-and-communication.md) for status updates, escalations, and risk management
   - Consult [Roles & Personas](./octoacme-roles-and-personas.md) to clarify responsibilities

## Questions or Feedback?

If you'd like to propose updates to these processes, use the [Add/Update Content to Process Docs](https://github.com/miguee-santana/skills-scale-institutional-knowledge-using-copilot-spaces/issues/new?template=add-update-content-to-process-docs.yml) issue template to request changes.
