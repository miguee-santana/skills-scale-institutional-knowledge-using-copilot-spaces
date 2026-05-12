# OctoAcme Decision Authority Matrix

## Purpose
Clarify decision rights and approval authority for each role to prevent ambiguity and bottlenecks.

## Decision Authority Framework

**Decision Levels:**
- **A (Authority):** Has final decision-making power
- **R (Responsible):** Owns the decision and is accountable
- **C (Consulted):** Provides input and feedback
- **I (Informed):** Notified of the decision after made

---

## Strategic & Scope Decisions

| Decision | PM | PdM | Product Lead | Sponsor | Tech Lead | QA Lead |
|----------|----|----|--------------|---------|-----------|---------|
| Project go/no-go (Initiation) | R | C | A | A | C | I |
| Roadmap prioritization | C | R | A | C | C | I |
| Feature scope for release | C | R | A | I | C | C |
| Major scope change (mid-project) | R | C | A | A | C | I |
| Release go/no-go | R | C | C | A | C | R |
| Cancellation or pause | I | C | A | A | I | I |

---

## Technical Decisions

| Decision | Tech Lead | Developers | PM | PdM | QA Lead |
|----------|-----------|-----------|----|----|---------|
| Technology/tool selection | A | C | I | I | C |
| Architecture approach | R | C | I | I | C |
| Code quality standards | A | R | I | I | C |
| Test coverage requirements | C | C | I | I | R |
| Performance requirements | R | C | C | C | C |
| Refactoring/technical debt | R | C | C | I | C |

---

## Execution & Timeline Decisions

| Decision | PM | PdM | Product Lead | Developers | Scrum Master |
|----------|----|----|--------------|-----------|--------------|
| Sprint backlog & tasks | C | I | I | R | R |
| Delivery timeline/dates | R | C | A | C | I |
| Resource allocation | R | I | C | C | C |
| Blocker escalation | R | C | A | I | C |
| Work-around vs. fix trade-off | R | C | A | C | I |
| Sprint velocity adjustment | C | I | I | R | R |

---

## Quality & Release Decisions

| Decision | QA Lead | Developers | PM | PdM | Tech Lead |
|----------|---------|-----------|----|----|-----------|
| Test strategy/approach | R | C | I | I | C |
| Acceptance criteria clarity | C | C | I | R | C |
| Bug severity & fix priority | R | I | C | C | C |
| Release readiness | R | I | C | C | C |
| Hotfix approval (production) | R | C | C | C | A |
| Post-release rollback | R | C | R | I | A |

---

## Communication & Escalation Decisions

| Decision | PM | Product Lead | Sponsor | Product Manager |
|----------|----|----|---------|-----------------|
| Stakeholder communication | R | C | I | C |
| Risk escalation | R | C | A | C |
| Bad news communication | R | I | A | C |
| Customer commitment | I | I | A | R |
| Public announcement | C | I | A | C |

---

## When in Doubt: Escalation Path

1. **Team Level:** Ask the role owner directly (check matrix above)
2. **Project Level:** Escalate to Project Manager
3. **Product Level:** Product Manager escalates to Product Lead
4. **Business Level:** Product Lead escalates to Sponsor

**Example Escalation Paths:**

- Bug severity disagreement: QA Lead → Project Manager → Product Lead
- Timeline concern: Developer → Scrum Master/PM → Product Lead → Sponsor
- Technical vs. business trade-off: Tech Lead → PM → Product Lead
- Strategic alignment: Product Manager → Product Lead → Sponsor

---

## Decision-Making Guidelines

### Speed vs. Consensus
- **Green light decisions (hire, yes to stakeholder):** Seek consensus; take time
- **Yellow light decisions (timeline, scope):** Consult broadly; PM decides with Product Lead
- **Red light decisions (cancel, major change):** Sponsor decides; consult others; communicate clearly

### Making Good Decisions
1. **Involve the right people:** Use RACI above
2. **Gather facts:** Don't decide without complete information
3. **Consider trade-offs:** Every decision has a cost; make trade-offs explicit
4. **Communicate clearly:** Why we decided, who decided, what happens next
5. **Iterate if needed:** Decisions can be revisited if new info emerges

### Reversing a Decision
- If a decision proves wrong, raise it immediately (don't wait for retrospective)
- Present new evidence or changed conditions
- Re-involve the original decision authority
- Communicate the change clearly to stakeholders

---

## Common Decision Scenarios

### Scenario 1: Scope Change Request (Mid-Sprint)

**Who decides:** Product Lead (with Sponsor approval if business-impacting)  
**Process:**
1. PdM + PM + Tech Lead + QA Lead meet to assess impact
2. PM calculates trade-off: what else slips if we add this?
3. Product Lead decides: yes, no, or defer to next sprint
4. PM communicates decision and updated timeline to Sponsor

---

### Scenario 2: Critical Bug Found in Production

**Who decides on fix:** QA Lead + Tech Lead + PM decide together  
**Who decides on timing:** PM (with escalation to Sponsor if affects customer SLA)  
**Process:**
1. QA Lead assesses severity and impact
2. Tech Lead assesses fix effort and risk
3. PM decides: hotfix now, patch in next release, or workaround?
4. If hotfix: coordinate with Sponsor for deployment window
5. Post-deployment: retrospective on how bug got to production

---

### Scenario 3: Two Features Competing for Priority

**Who decides:** Product Lead  
**Process:**
1. PdM prepares impact analysis for each feature
2. PM estimates effort and timeline impact
3. Product Lead makes decision based on strategic fit
4. PdM + PM update backlog and communicate decision

---

### Scenario 4: Team Concerned About Quality

**Who decides on process change:** Scrum Master + Team (Agile consensus)  
**Who approves time allocation:** PM + Product Lead  
**Process:**
1. Scrum Master / team raises concern in retrospective
2. Team proposes solution (e.g., increase test time, add code review)
3. PM assesses time/timeline impact
4. Product Lead approves if it affects delivery timeline
5. Implement and measure impact in next sprint

---

## Preventing Decision Bottlenecks

### Problem: Decisions Take Too Long

**Root Causes:**
- Waiting for consensus when authority is clear
- Unclear who should decide
- Missing information delays decision

**Solutions:**
- Use this matrix to clarify authority upfront
- Set decision deadlines (e.g., "decide by EOD tomorrow")
- Empower lower levels to decide when low-risk (e.g., backlog prioritization)

### Problem: Reversals Cause Confusion

**Root Causes:**
- Decision not communicated clearly
- Decision authority unclear to team
- New information emerges later

**Solutions:**
- Always explain the "why" when communicating decisions
- Document decision rationale in decision log
- Create psychological safety to revisit decisions with new info

### Problem: Escalation Happens Too Late

**Root Causes:**
- Team tries to solve issues they can't resolve
- Escalation path unclear
- Fear of escalating up

**Solutions:**
- Set clear criteria for when to escalate (e.g., "if it changes timeline or scope")
- Normalize escalation as good communication
- Review escalation patterns in retrospectives

---

## Related Documents
- `octoacme-roles-and-personas.md` – Full role definitions and interactions
- `role-assignment-guide.md` – When to assign each role
- `octoacme-project-management-overview.md` – OctoAcme principles and lifecycle
