# Open-LMX Actor Model

## Purpose

The Open-LMX Platform connects actors across the education-to-employment ecosystem.

Each actor has different responsibilities, incentives, permissions, data ownership boundaries, and workflows.

## Primary Actors

```text
Learner
Student
Worker
Instructor
Mentor
Educational Institution
Training Provider
Certification Body
Employer
Recruiter
Hiring Manager
Industry Body
Government or Workforce Agency
Verifier
Platform Administrator
```

## Actor: Learner

A learner is any person building knowledge, skills, competencies, credentials, and career capability.

Responsibilities:

- Own learning profile
- Consent to share records
- Complete learning activities
- Complete assessments
- Collect credentials
- Build evidence portfolio

Needs:

- Portable skill profile
- Learning path recommendations
- Verified credentials
- Job readiness visibility
- Career guidance

## Actor: Student

A student is a learner associated with an educational institution.

Responsibilities:

- Participate in curriculum
- Complete institutional assessments
- Build verified academic and skill records

Needs:

- Institution-linked learning record
- Industry-aligned skill map
- Employability visibility

## Actor: Worker

A worker is a learner with work experience and career history.

Responsibilities:

- Maintain skill and work evidence
- Keep credentials current
- Track growth and performance

Needs:

- Career progression paths
- Reskilling paths
- Role readiness mapping

## Actor: Instructor

An instructor creates, delivers, or evaluates learning.

Responsibilities:

- Create learning resources
- Map lessons to outcomes
- Assess learners
- Provide feedback

Needs:

- Course authoring tools
- Rubric management
- Outcome tracking
- Learner progress visibility

## Actor: Mentor

A mentor supports learner growth and career development.

Responsibilities:

- Guide learners
- Review progress
- Recommend learning or projects

Needs:

- Learner capability view
- Growth plan visibility
- Recommendation workflows

## Actor: Educational Institution

An institution publishes education programs, courses, assessments, and verified learner records.

Responsibilities:

- Publish curriculum
- Map courses to competencies
- Issue institutional records
- Track employability outcomes

Needs:

- Curriculum-to-skill mapping
- Student outcome analytics
- Employer alignment signals
- Credential issuance workflows

## Actor: Training Provider

A training provider offers learning and skilling programs outside or alongside formal education.

Responsibilities:

- Publish training programs
- Map programs to skills and roles
- Provide assessments and completion records

Needs:

- Course registry
- Skill alignment
- Credential issuance
- Employer demand analytics

## Actor: Certification Body

A certification body verifies skills, competencies, capabilities, or professional standards.

Responsibilities:

- Define certification criteria
- Run or approve assessments
- Issue and revoke credentials
- Maintain verification rules

Needs:

- Credential registry
- Verification APIs
- Revocation workflows
- Trust and compliance reporting

## Actor: Employer

An employer defines work demand and consumes verified capability signals.

Responsibilities:

- Publish roles and jobs
- Define capability requirements
- Evaluate candidates
- Provide hiring and performance feedback

Needs:

- Role-to-skill mapping
- Candidate capability verification
- Work readiness scoring
- Skill-gap analytics

## Actor: Recruiter

A recruiter connects candidates to roles using structured, trusted signals.

Responsibilities:

- Search candidate profiles
- Screen against role requirements
- Coordinate hiring workflows

Needs:

- Evidence-backed candidate profiles
- Structured matching
- Reduced keyword dependence
- Trust and verification indicators

## Actor: Hiring Manager

A hiring manager evaluates role fit and makes hiring decisions.

Responsibilities:

- Define practical role expectations
- Review evidence and interviews
- Make hiring recommendations

Needs:

- Capability fit view
- Evidence summary
- Interview evaluation support
- Skill gap visibility

## Actor: Industry Body

An industry body defines sector capability expectations and standards.

Responsibilities:

- Define skill and competency frameworks
- Publish occupation models
- Align industry needs with education

Needs:

- Sector skill maps
- Workforce readiness analytics
- Standard publishing workflows

## Actor: Government or Workforce Agency

A government or workforce agency supports policy, workforce planning, and public-good skilling.

Responsibilities:

- Track workforce readiness
- Define policy programs
- Support public skilling initiatives

Needs:

- Aggregated skill gap analytics
- Credential trust frameworks
- Institution and employer alignment views

## Actor: Verifier

A verifier checks whether a credential, claim, profile, or evidence artifact is valid.

Responsibilities:

- Verify claims
- Validate credentials
- Check revocation status

Needs:

- Verification APIs
- Evidence references
- Trust status

## Actor: Platform Administrator

A platform administrator manages commercial platform operations.

Responsibilities:

- Manage tenants
- Configure governance
- Monitor services
- Handle audits
- Operate integrations

Needs:

- Admin console
- Audit logs
- Policy controls
- Operational dashboards

## Actor Relationship Graph

```text
Learner
  earns Credential
  demonstrates Competency
  builds Capability
  applies_to Job

Institution
  publishes Course
  assesses Learner
  issues Record

Employer
  defines Role
  requires Capability
  evaluates Candidate

Recruiter
  matches Candidate to Role

Certification Body
  certifies Competency
  verifies Credential

Industry Body
  defines Skill Framework
  informs Curriculum

Government
  observes Workforce Readiness
  supports Skilling Programs
```

## Platform Design Rule

Every actor must have clear ownership, consent, permissions, responsibilities, and auditability.

No actor should gain access to learner evidence, credentials, or profile data without appropriate authorization and consent.
