# OctoAcme Personas

This document defines typical roles and responsibilities used in OctoAcme project docs and exercises.

---

## Developers

### Role Summary
Developers design, build, test, and deliver software components. They collaborate with product and project leads to implement features that meet acceptance criteria and quality standards.

### Responsibilities
- Implement features and fixes to meet acceptance criteria
- Write and maintain tests and documentation
- Participate in design and code reviews
- Assist in estimating and planning work
- Help identify technical risks and propose mitigations

### Goals
- Deliver reliable, maintainable code
- Reduce cycle time from idea to production
- Maintain high test coverage and observability

### Typical Communication
- Daily standups and sprint planning
- PR descriptions and code review comments
- Technical design docs when needed

---

## Product Managers

### Role Summary
Product Managers define what should be built to deliver customer and business value. They own the product vision, prioritize the backlog, and measure outcomes.

### Responsibilities
- Define problem statements and success metrics
- Prioritize the roadmap and backlog
- Collaborate with stakeholders and engineering on trade-offs
- Validate solutions through user research and metrics

### Goals
- Maximize customer value and impact
- Make clear, data-driven prioritization decisions
- Ensure product-market fit and usability

### Typical Communication
- Weekly alignment with PM and engineering leads
- Roadmap updates and stakeholder briefings
- Acceptance criteria and feature specs

---

## Project Managers

### Role Summary
Project Managers coordinate delivery activities, manage schedules, risks, and communications. They enable the team to deliver on commitments efficiently.

### Responsibilities
- Create and maintain project plans and timelines
- Manage risks, dependencies, and resource constraints
- Facilitate meetings (kickoff, planning, retrospectives)
- Ensure consistent project documentation and status reporting
- Coordinate cross-team and stakeholder communication

### Goals
- Deliver projects on time and within scope
- Minimize unplanned work and escalations
- Maintain transparency and alignment across stakeholders

### Typical Communication
- Weekly status updates and stakeholder reports
- Risk registers and decision logs
- Coordination via project boards and meeting facilitation

---

## UX / Design Lead

### Role Summary
The UX/Design Lead owns the user experience, interface design, and accessibility standards for the product. They translate customer needs and product requirements into intuitive, visually consistent designs and validate that implementations match the intended experience before release.

### Responsibilities
- Create wireframes, prototypes, and high-fidelity designs aligned to product requirements
- Define and maintain a shared design system and component library
- Conduct usability research and incorporate findings into design iterations
- Review implementations against design specifications and raise quality issues
- Ensure accessibility standards (WCAG) are met for all user-facing features

### Goals
- Deliver a consistent, accessible, and delightful user experience
- Reduce design-to-development handoff friction
- Build shared design language across product teams

### Typical Communication
- Design reviews with Developers and Product Managers before and during sprints
- Usability findings shared as research reports or issue comments
- Participation in sprint demos to evaluate UI fidelity

### Interactions with existing roles
- Collaborates with **Product Manager** to align designs with product goals and acceptance criteria
- Works with **Developers** during implementation to resolve design questions and review PRs with UI changes
- Coordinates with **Project Manager** on design milestone timelines and dependencies

---

## Engineering Manager / Tech Lead

### Role Summary
The Engineering Manager (EM) or Tech Lead provides technical direction, mentors developers, owns architectural decisions, and is accountable for the health and productivity of the engineering team. In smaller teams these responsibilities may be held by a single Tech Lead; in larger teams they may be split.

### Responsibilities
- Define and communicate architectural standards and technical direction
- Review and approve significant technical decisions (ADRs, infrastructure changes)
- Conduct code reviews for complex or high-risk changes
- Mentor developers and support career growth
- Partner with the Project Manager on capacity planning and unblocking delivery
- Own technical debt backlog and advocate for engineering quality investments

### Goals
- Maintain a high-quality, sustainable codebase
- Grow engineering team capability and retention
- Align technical decisions with product and business objectives

### Typical Communication
- Architecture decision reviews and technical design docs
- 1:1s with developers and participation in engineering team meetings
- Escalation point for technical blockers during PM/delivery syncs

### Interactions with existing roles
- Partners with **Product Manager** to evaluate technical feasibility and trade-offs
- Works with **Project Manager** on scheduling, capacity, and dependency management
- Supports **Developers** by unblocking technical decisions and providing mentorship

---

## Security Engineer

### Role Summary
The Security Engineer reviews code and infrastructure for vulnerabilities, owns the security scanning configuration in CI/CD, and serves as the sign-off authority for security gates in the release process. They also respond to security incidents and drive blameless post-mortems.

### Responsibilities
- Configure and maintain security scanning tools in CI (SAST, dependency scanning, secret detection)
- Review high-risk features (auth, permissions, data handling) before release
- Maintain a threat model for key product surfaces
- Respond to security incidents following the security incident runbook
- Provide security guidance and training to development teams

### Goals
- Minimize vulnerability exposure in production
- Shift security left — catch issues in development, not in production
- Maintain compliance with applicable standards and policies

### Typical Communication
- Security review comments on PRs and design docs
- Pre-release sign-off in the deployment checklist
- Incident triage communications and post-incident reports

### Interactions with existing roles
- Works with **Developers** and **Engineering Manager** to remediate vulnerabilities and adopt secure coding patterns
- Partners with **Project Manager** to schedule security reviews into the release timeline
- Coordinates with **Product Manager** on compliance and privacy requirements that affect feature design

---

## Data Analyst

### Role Summary
The Data Analyst tracks the success metrics defined in project one-pagers, builds dashboards and reports, and surfaces data insights that inform Product Manager prioritization and stakeholder communication.

### Responsibilities
- Instrument features with appropriate logging and analytics events
- Build and maintain dashboards for key product and operational metrics
- Produce post-release impact reports tied to defined success metrics
- Identify anomalies, trends, or regressions in usage and performance data
- Support A/B testing and experimentation analysis

### Goals
- Provide reliable, timely data to support decision-making
- Reduce the time from data question to actionable insight
- Ensure metric definitions are consistent and well-documented

### Typical Communication
- Weekly metric reviews with Product Manager and Project Manager
- Dashboard links included in release notes and status reports
- Ad-hoc analysis shared via issue comments or short reports

### Interactions with existing roles
- Partners with **Product Manager** to define success metrics and interpret results
- Works with **Developers** to ensure correct event instrumentation
- Provides data to **Project Manager** for burndown, velocity, and milestone reporting

---

## Customer Success / Support Representative

### Role Summary
The Customer Success or Support Representative is the voice of the customer within the project team. They surface customer pain points from support queues and feedback channels, review release notes before publication, and coordinate communication to customers and support staff when changes ship.

### Responsibilities
- Surface trending customer issues and feedback to Product Manager during planning
- Review release notes and changelogs for clarity and customer impact before publication
- Coordinate customer-facing communications for significant releases or breaking changes
- Document known issues and workarounds for the support knowledge base
- Escalate critical customer-impacting issues to the PM and Product Lead

### Goals
- Minimize customer disruption from product changes
- Reduce support ticket volume through proactive communication and documentation
- Ensure the support team is prepared for every release

### Typical Communication
- Pre-release briefings with the Product Manager and Project Manager
- Release note reviews before deployment
- Post-release monitoring of support ticket trends and feedback loops

### Interactions with existing roles
- Partners with **Product Manager** to prioritize customer-reported bugs and friction points
- Works with **Project Manager** to ensure customer communications are included in the release checklist
- Collaborates with **Developers** to validate workarounds and document known issues accurately

---

## QA Lead

### Role Summary
The QA Lead owns the testing strategy for the project, coordinates manual and automated QA efforts, and ensures the Definition of Done includes appropriate quality gates before any increment ships to production.

### Responsibilities
- Define and maintain the overall test plan and QA approach for each project
- Coordinate automated and manual test coverage across unit, integration, and end-to-end layers
- Review acceptance criteria on backlog items to confirm they are testable
- Sign off on release readiness from a quality perspective
- Track and report defect trends and test coverage metrics

### Goals
- Prevent regressions from reaching production
- Shift quality assurance left into development workflows
- Maintain clear, repeatable quality gates for every release

### Typical Communication
- Participates in sprint planning to validate acceptance criteria and testability
- Reports defect status and test coverage in weekly delivery syncs
- Provides QA sign-off in the release deployment checklist

### Interactions with existing roles
- Works with **Developers** to define testable acceptance criteria and review automated test coverage
- Partners with **Project Manager** to schedule QA milestones and raise quality-related blockers
- Coordinates with **Security Engineer** on security test coverage and vulnerability remediation validation

---

## Release Manager

### Role Summary
The Release Manager oversees release readiness, coordinates deployments across teams, maintains changelogs, and ensures all pre-release requirements are met before any version ships. They are the single point of accountability for the deployment checklist.

### Responsibilities
- Own and execute the deployment checklist for each release
- Coordinate release windows with engineering, operations, and stakeholder teams
- Maintain release notes and changelogs aligned to each release type (patch, minor, major)
- Manage rollback decisions in collaboration with Engineering Manager and on-call teams
- Track release history and post-deploy verification results

### Goals
- Reduce deployment risk through consistent, documented release processes
- Ensure all stakeholders are informed and prepared for each release
- Minimize time-to-recovery when releases require rollback

### Typical Communication
- Pre-release readiness reviews with QA Lead, Security Engineer, and Project Manager
- Deployment status updates to stakeholders during release windows
- Post-release retrospective items raised for any deployment incidents

### Interactions with existing roles
- Partners with **Project Manager** to align release timelines with project milestones
- Works with **QA Lead** and **Security Engineer** to confirm all quality and security gates are cleared
- Coordinates with **Customer Success / Support Representative** on customer-facing communications before and after each release

---

## Business Analyst

### Role Summary
The Business Analyst bridges requirements from business stakeholders into clear, actionable backlog items. They work alongside the Product Manager and Project Manager to ensure technical teams have the context needed to implement the right solution.

### Responsibilities
- Elicit, document, and validate requirements from business stakeholders
- Translate business needs into well-formed user stories with acceptance criteria
- Facilitate requirements workshops and stakeholder alignment sessions
- Maintain traceability between business objectives and backlog items
- Identify and flag scope creep or requirement conflicts early

### Goals
- Reduce ambiguity in backlog items before they enter a sprint
- Ensure implemented solutions map directly to stated business needs
- Improve handoff quality between business stakeholders and delivery teams

### Typical Communication
- Requirements workshops and stakeholder interviews
- Written user stories and process flow documentation shared with delivery teams
- Participation in sprint planning to clarify requirements and answer questions

### Interactions with existing roles
- Pairs closely with **Product Manager** to align business requirements with product vision and prioritization
- Works with **Project Manager** to surface dependency and scope risks early
- Collaborates with **Developers** during sprint planning to clarify acceptance criteria and resolve ambiguity

---

## How these personas are used in the exercise
- Use these persona definitions to frame scenarios and sample interactions in the Skills Exercise.
- Each persona can be used as a persona prompt for Copilot Spaces to shape role-specific guidance.

