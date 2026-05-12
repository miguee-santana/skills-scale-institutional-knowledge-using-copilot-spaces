# OctoAcme Role Assignment Guide

## Purpose
Provide guidance on when to assign each role and what responsibilities they own during different project phases.

## Role Assignment by Project Phase

### Initiation Phase

**When:** Project idea is ready to explore or validate  
**Duration:** 1–2 weeks typically

**Required Roles:**
- **Product Manager:** Define problem statement and success metrics
- **Project Manager:** Create One-pager and stakeholder list, schedule kickoff
- **Product Lead:** Review One-pager and provide strategic context

**Optional Roles:**
- **Sponsor/Stakeholder:** Validate business need and provide approval (gate decision)
- **Technical Lead:** Assess technical feasibility for key assumptions
- **Developers:** Advisory input on effort estimates (optional)

**Key Deliverable:** Project One-pager + approval to move to planning

---

### Planning Phase

**When:** Project approved for planning  
**Duration:** 1–4 weeks depending on scope

**Required Roles:**
- **Product Manager:** Prioritize backlog, define acceptance criteria
- **Project Manager:** Create project plan, schedule, and dependencies
- **Developers:** Estimate work, identify technical risks
- **QA/Testing Lead:** Define test strategy and acceptance testing approach
- **Technical Lead:** Review architecture and technical approach

**Optional Roles:**
- **Scrum Master:** Facilitate planning sessions if using Scrum
- **Product Lead:** Review prioritization trade-offs
- **Sponsor:** Validate timeline and resource plan

**Key Deliverables:** Prioritized backlog, sprint plan, test plan, risk register

---

### Execution Phase

**When:** Team begins building  
**Duration:** Multiple sprints until release

**Required Roles:**
- **Developers:** Implement features to acceptance criteria
- **Product Manager:** Clarify acceptance criteria, validate features
- **Project Manager:** Track progress, manage risks, escalate blockers
- **QA/Testing Lead:** Run tests, validate acceptance criteria, report quality metrics
- **Scrum Master:** Facilitate standups and sprints, support team

**Optional Roles:**
- **Technical Lead:** Design reviews, technical mentoring
- **Product Lead:** Escalation for prioritization/trade-off decisions

**Key Metrics:** Velocity, burndown, test coverage, bug count, cycle time

---

### Release Phase

**When:** Features ready for production deployment  
**Duration:** 1–3 days typically

**Required Roles:**
- **Project Manager:** Coordinate release schedule and communications
- **QA/Testing Lead:** Validate release readiness through smoke tests
- **Developers:** Deploy code and support in-flight issues

**Optional Roles:**
- **Product Manager:** Draft release notes and customer messaging
- **Technical Lead:** Technical readiness validation
- **Sponsor:** Go/no-go approval for production deployment
- **Product Lead:** Go/no-go approval if strategic concerns

**Key Deliverables:** Release notes, deployment verification, post-release monitoring

---

### Retrospective & Close Phase

**When:** After each sprint, release, or major milestone  
**Duration:** 60–90 minutes

**Required Roles:**
- **Scrum Master:** Facilitate retrospective and capture action items
- **Project Manager:** Summarize project outcomes and lessons learned
- **Product Manager:** Share outcome metrics and learnings
- **Developers:** Provide technical learnings and process feedback
- **QA/Testing Lead:** Report on quality outcomes

**Optional Roles:**
- **Product Lead:** High-level retrospective for strategic projects
- **Sponsor:** Close meeting for executive visibility

**Key Deliverables:** Retrospective notes, action items, lessons learned, project closure

---

## Role Sizing Guidelines

### When do you need a full-time dedicated person?

| Role | Project Size | Needed When |
|------|--------------|------------|
| **PM** | Any | Always (core coordinator) |
| **PdM** | Med/Large | Features requiring prioritization; customer input |
| **Tech Lead** | Large | Multiple teams or complex architecture |
| **QA Lead** | Large | High-risk features; compliance requirements |
| **Scrum Master** | Any | If practicing Scrum; essential for team velocity |
| **Sponsor** | Any | Required for go/no-go gates; advisory otherwise |

### When can a role be part-time or shared?

- **Product Lead:** Typically advisory; escalation authority only when needed
- **Technical Lead:** Can split across 2–3 projects if architecture is stable
- **Sponsor:** Part-time; primarily involved at gates and escalations

---

## Escalation & Decision Clarity

### Who decides what?

- **Product priorities:** Product Manager (with Product Lead approval for strategic trade-offs)
- **Timeline/scope:** Project Manager (with Sponsor approval if business-impacting)
- **Technical approach:** Technical Lead (with team input)
- **Quality/release readiness:** QA Lead + Project Manager
- **Strategic direction:** Product Lead + Sponsor

See `docs/decision-authority-matrix.md` for detailed decision rights.

---

## Onboarding Checklist for Each Role

### Product Manager
- [ ] Review current roadmap and backlog
- [ ] Understand customer segments and success metrics
- [ ] Align with Product Lead on priorities
- [ ] Schedule weekly PM sync

### Project Manager
- [ ] Review project charter and timeline
- [ ] Set up project board and communication channels
- [ ] Schedule kickoff with team
- [ ] Configure risk register and status reporting

### Developers
- [ ] Review codebase and dev environment setup
- [ ] Understand acceptance criteria and Definition of Done
- [ ] Join daily standups
- [ ] Pair with experienced team member on first task

### QA/Testing Lead
- [ ] Review existing test strategy and coverage
- [ ] Understand acceptance criteria and user workflows
- [ ] Set up test automation framework if needed
- [ ] Coordinate test plan with developers

### Technical Lead
- [ ] Review architecture and technical strategy
- [ ] Understand technical constraints and tech debt
- [ ] Schedule design review cadence
- [ ] Align with Product Lead on technical priorities

### Scrum Master
- [ ] Understand team composition and dynamics
- [ ] Review retrospective history and action items
- [ ] Set up sprint ceremonies and timebox them
- [ ] Establish blocker escalation process

---

## Common Anti-Patterns to Avoid

❌ **"Everyone's a PM"** – No clear accountability for project coordination  
✅ **Better:** One designated PM; others are stakeholders and contributors

❌ **"We don't have a QA Lead"** – Quality issues caught too late in production  
✅ **Better:** Assign QA responsibility even if part-time

❌ **"Tech Lead decides everything"** – Slows down developers and reduces ownership  
✅ **Better:** Tech Lead reviews designs; developers have autonomy on implementation

❌ **"No retrospectives"** – Team repeats the same mistakes every sprint  
✅ **Better:** Retrospectives with action item tracking (Scrum Master's job)

❌ **"Sponsor involved in details"** – Wastes executive time and creates bottlenecks  
✅ **Better:** Sponsor involved at gates; PM escalates blockers as needed

---

## Related Documents
- `octoacme-roles-and-personas.md` – Full persona definitions and interactions
- `decision-authority-matrix.md` – Detailed decision rights for each role
- `octoacme-project-management-overview.md` – OctoAcme principles and lifecycle
