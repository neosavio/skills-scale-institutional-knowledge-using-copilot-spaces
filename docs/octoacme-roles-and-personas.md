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

## QA Lead

<!-- Fits into: Execution (test planning/sign-off), Release (readiness gate), and Retrospective phases -->

### Role Summary
The QA Lead oversees the quality strategy for the project, defines test plans, and ensures that quality gates are enforced before releases. They act as the primary voice for quality across all delivery phases.

### Responsibilities
- Develop and communicate test plans covering unit, integration, and end-to-end testing
- Coordinate manual and automated testing activities with Developers
- Review acceptance criteria and Definition of Done to ensure testability
- Escalate critical defects and blocking issues to the Project Manager and relevant Developers
- Sign off on release readiness in collaboration with the Release Manager
- Maintain a defect log and track resolution progress

### Goals
- Prevent regressions and maintain quality standards across all releases
- Shift quality left by engaging early in planning and design
- Provide clear pass/fail signals at each quality gate

### Typical Communication
- Participates in sprint planning to review acceptance criteria
- Provides QA status updates during standups and weekly syncs
- Issues release-readiness sign-off to the Release Manager before deployment
- Collaborates with Developers via defect tickets and PR review comments

### Interactions
- **Developers:** Reviews pull requests for test coverage; pairs on reproducing and resolving defects
- **Project Manager:** Reports QA blockers, timeline risks, and overall test progress
- **Product Manager:** Validates that features meet acceptance criteria and usability expectations
- **Release Manager:** Provides formal release-readiness sign-off; raises concerns about unresolved critical issues

---

## UX/UI Designer

<!-- Fits into: Initiation (requirements gathering/user research), Planning (design assets), and Execution (design review) phases -->

### Role Summary
The UX/UI Designer ensures that deliverables meet usability standards and align with user experience guidelines. They translate user needs and product requirements into wireframes, mockups, and production-ready design assets.

### Responsibilities
- Conduct user research and usability testing to inform design decisions
- Create wireframes, mockups, prototypes, and final visual design assets
- Participate in requirements gathering sessions alongside the Product Manager
- Validate designs with the Product Manager before handoff to Developers
- Provide design review feedback during development to ensure implementation fidelity
- Maintain a shared design system or style guide for consistency

### Goals
- Deliver intuitive, accessible, and visually consistent user experiences
- Reduce development rework by providing clear, annotated design handoffs
- Advocate for the end user throughout the project lifecycle

### Typical Communication
- Design reviews with Product Manager and Developers at key milestones
- Handoff documentation (see `docs/octoacme-design-handoff-checklist.md`) shared with developers
- Participates in retrospectives to identify UX-related improvements

### Interactions
- **Product Manager:** Aligns on user stories, success metrics, and acceptance criteria; validates final designs
- **Developers:** Delivers annotated mockups and assets; answers implementation questions during execution
- **QA Lead:** Shares design specs to support visual/functional testing
- **Customer Support Lead:** Incorporates common user pain points and feedback into design iterations

---

## Release Manager

<!-- Fits into: Release & Deployment phase, with coordination spanning Planning and Execution -->

### Role Summary
The Release Manager owns the release workflow and coordinates all deployment activities. They ensure releases are planned, communicated, and executed with minimal risk and maximum transparency.

### Responsibilities
- Schedule, document, and coordinate release windows across teams
- Maintain release plans, change logs, and rollback procedures
- Communicate release status, timelines, and any issues to stakeholders
- Verify that pre-release requirements (CI passing, QA sign-off, release notes) are met before deployment
- Facilitate post-release reviews and capture action items for improvement
- Manage the release checklist (see `docs/octoacme-release-checklist.md`)

### Goals
- Deliver stable, well-communicated releases on schedule
- Reduce release-related incidents through rigorous pre-release checks
- Build a repeatable, low-friction release process

### Typical Communication
- Release schedule and change notifications sent to all stakeholders
- Pre-release readiness reviews with QA Lead and Developers
- Post-release retrospective summary shared with Project Manager and Product Manager

### Interactions
- **Project Manager:** Coordinates release windows within the overall project timeline; escalates blockers
- **Developers:** Confirms deployment artifacts, pipeline readiness, and hotfix procedures
- **QA Lead:** Receives release-readiness sign-off before initiating deployment
- **Customer Support Lead:** Provides advance notice of releases and known issues for support preparation

---

## Customer Support Lead

<!-- Fits into: Release (post-release support) and Retrospective phases; also feeds back into Planning via user pain points -->

### Role Summary
The Customer Support Lead acts as the liaison between end users and the project team. They capture, triage, and escalate user-reported issues and ensure that recurring pain points are translated into actionable feedback for the backlog.

### Responsibilities
- Gather and triage incoming support requests and user-reported issues
- Translate common user pain points into clearly articulated feedback items for the Product Manager
- Coordinate post-release support coverage, including training and FAQ updates
- Escalate critical user-facing bugs to Developers and the QA Lead
- Track issue resolution timelines and communicate status back to affected users
- Contribute to onboarding materials to reduce repeat support requests

### Goals
- Minimize the time-to-resolution for user-facing issues
- Close the feedback loop between end users and the delivery team
- Reduce repeat contacts through proactive documentation and training

### Typical Communication
- Provides a weekly support summary (top issues, trends, resolutions) to the Product Manager
- Participates in post-release reviews to share early user feedback
- Collaborates with Technical Writer to keep help documentation accurate and current

### Interactions
- **Product Manager:** Feeds user pain points and trends into backlog prioritisation decisions
- **Developers:** Escalates critical bugs with reproducible steps; tracks fix status
- **QA Lead:** Shares user-reported defects for triage and regression testing
- **Release Manager:** Receives advance release notes to prepare support teams and documentation
- **Technical Writer:** Partners to keep end-user documentation and FAQs up to date

---

## Technical Writer

<!-- Fits into: all phases — documents outputs at Initiation, Planning, Execution, Release, and Retrospective -->

### Role Summary
The Technical Writer documents key workflows, features, and release notes for both internal and external audiences. They maintain consistency and clarity across all project documentation artifacts.

### Responsibilities
- Create and update process documentation, onboarding guides, and user-facing help content
- Work with Product Manager and Developers to accurately document new features at each release
- Review all project artifacts for consistency in terminology, formatting, and completeness
- Produce release notes and changelogs in collaboration with the Release Manager
- Maintain a documentation style guide and template library (see `docs/` folder)

### Goals
- Ensure all project stakeholders have access to accurate, up-to-date documentation
- Reduce onboarding time for new team members through clear, well-structured guides
- Establish and enforce documentation standards across the project

### Typical Communication
- Regular syncs with Product Manager and Developers to capture feature details
- Reviews documentation pull requests and raises consistency issues
- Provides updated docs alongside each release for the Release Manager and Customer Support Lead

### Interactions
- **Product Manager:** Receives feature specs and success criteria to incorporate into user documentation
- **Developers:** Gathers technical details about implementation, APIs, and configuration
- **Release Manager:** Delivers release notes and changelog entries as part of the release process
- **Customer Support Lead:** Keeps end-user help articles aligned with current product behaviour
- **QA Lead:** Reviews test plans and QA artifacts to ensure documentation completeness

---

## How these personas are used in the exercise
- Use these persona definitions to frame scenarios and sample interactions in the Skills Exercise.
- Each persona can be used as a persona prompt for Copilot Spaces to shape role-specific guidance.
- New roles (QA Lead, UX/UI Designer, Release Manager, Customer Support Lead, Technical Writer) participate across multiple phases of the project lifecycle; see `docs/octoacme-project-management-overview.md` for the full lifecycle overview.

