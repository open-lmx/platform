# Open-LMX Platform Architecture

## Purpose

Open-LMX Platform is the commercial implementation of the Open-LMX education-to-employment operating model.

The platform uses the open source Open-LMX Foundation as the shared standard layer, then adds hosted services, workflows, integrations, verification, analytics, governance, and support.

## Architecture Principle

Foundation defines the language.
Platform delivers the outcomes.

```text
Open-LMX Foundation
  -> data models
  -> schemas
  -> vocabulary
  -> governance
  -> interoperability contracts

Open-LMX Platform
  -> services
  -> APIs
  -> workflows
  -> portals
  -> integrations
  -> analytics
  -> verification
  -> managed operations
```

## Core Platform Graphs

The platform operates across five connected graphs:

```text
Knowledge Graph
Learning Graph
Capability Graph
Employment Graph
Career Graph
```

Together they support the full education-to-employment lifecycle:

```text
Knowledge
    ↓
Learning
    ↓
Assessment
    ↓
Competency
    ↓
Credential
    ↓
Capability
    ↓
Work Readiness
    ↓
Employment
    ↓
Career Progression
    ↓
Trust
```

## Bounded Contexts

### 1. Knowledge Service

Manages governed knowledge assets.

Responsibilities:

- Concepts
- Terms
- Definitions
- Frameworks
- Taxonomies
- Knowledge graph relationships

### 2. Learning Service

Manages learning assets.

Responsibilities:

- Learning resources
- Courses
- Modules
- Lessons
- Learning paths
- Curriculum alignment

### 3. Assessment Service

Manages evidence-producing evaluation activities.

Responsibilities:

- Assessments
- Questions
- Rubrics
- Attempts
- Submissions
- Scores
- Feedback

### 4. Competency Service

Maps learning and assessment evidence to skills, competencies, and capabilities.

Responsibilities:

- Skills
- Competencies
- Proficiency levels
- Capability requirements
- Evidence mapping

### 5. Credential Service

Manages credentials and verification.

Responsibilities:

- Certificates
- Badges
- Credentials
- Issuance
- Verification
- Revocation
- Renewal

### 6. Profile Service

Manages learner, worker, institution, employer, and recruiter profiles.

Responsibilities:

- Learner profiles
- Worker profiles
- Institution profiles
- Employer profiles
- Recruiter profiles
- Consent and sharing preferences

### 7. Employment Service

Models work demand.

Responsibilities:

- Industries
- Occupations
- Roles
- Jobs
- Tasks
- Responsibilities
- Skill requirements
- Competency requirements
- Work readiness requirements

### 8. Matching Service

Connects capability supply to work demand.

Responsibilities:

- Candidate-role matching
- Skill gap matching
- Learning path recommendations
- Career path recommendations

### 9. Career Service

Supports growth and progression.

Responsibilities:

- Career paths
- Career levels
- Promotion paths
- Development plans
- Mentorship paths

### 10. Trust Service

Computes and exposes trust signals.

Responsibilities:

- Verification status
- Evidence quality
- Credential trust
- Institution trust
- Employer trust
- Assessment trust
- Capability confidence

### 11. Governance Service

Provides platform-level controls.

Responsibilities:

- Policy enforcement
- Audit trails
- Approval workflows
- Data access governance
- Consent governance
- Compliance reporting

### 12. Registry Service

Publishes discoverable assets.

Responsibilities:

- Skill registry
- Credential registry
- Institution registry
- Employer registry
- Course registry
- Assessment registry
- Role registry

## Commercial Application Surfaces

The platform should expose role-specific applications:

- Learner Portal
- Institution Portal
- Employer Portal
- Recruiter Portal
- Certification Body Portal
- Government or Workforce Agency Portal
- Admin Console

## API Strategy

The platform should expose:

- Public read APIs for registry discovery
- Authenticated APIs for profile and evidence exchange
- Enterprise APIs for integrations
- Verification APIs for credentials and claims
- Analytics APIs for reporting and workforce intelligence

## Integration Strategy

The platform should integrate with:

- Learning Management Systems
- Student Information Systems
- HRMS
- ATS
- Job boards
- Credential wallets
- Assessment tools
- Identity providers
- Government workforce systems

## Data Governance Principles

- Foundation schemas are the source of truth for interoperable models.
- Platform data must preserve provenance.
- Learner consent is required for profile sharing.
- Credentials must be verifiable.
- Assessments must preserve evidence.
- Matching decisions must be explainable.
- Audit trails must be retained.

## Initial Implementation Sequence

```text
1. Registry Service
2. Profile Service
3. Learning Service
4. Competency Service
5. Credential Service
6. Employment Service
7. Matching Service
8. Trust Service
9. Governance Service
10. Analytics and Reporting
```

## Strategic Moat

The commercial moat is not the schema itself.

The moat is:

- Verified network data
- Trust graph
- Skill and role intelligence
- Institution-employer workflows
- Enterprise integrations
- Evidence-backed matching
- Managed governance
- Analytics and reporting
- Operational reliability
