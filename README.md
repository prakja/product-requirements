# Product Requirements

Issue-tracker only — this repo holds **no code**. Every requirement lives here as a
complete PRD, produced by `/autonomous-wayfinder` or written by hand from the
[PRD template](.github/ISSUE_TEMPLATE/prd.md).

## Shape of a PRD

```
PRD issue                      label: prd
├── Epic issue                 label: epic        child of the PRD
│   └── User-story issue       label: user-story  child of the epic
│       ├── Acceptance criteria
│       ├── Functional requirements
│       └── Non-functional requirements
└── Epic issue
```

## The five elements

- **Epic**: A large body of work that can be broken down into smaller, targeted
  tasks. Epics often span multiple releases or sprints.
- **User Story**: A high-level description of a product feature, written from the
  perspective of the end user. It focuses on the who, what, and why of a feature.
- **Acceptance Criteria (AC)**: A set of predefined conditions or pass/fail
  requirements that a user story must meet to be considered complete ("Done").
- **Functional Requirements**: Descriptions of the specific behaviors, data
  processing, and functions the system must perform (e.g. "The system must send a
  verification email upon signup").
- **Non-Functional Requirements (NFRs)**: Criteria that specify how a system
  should perform rather than what it does — scalability, security, performance,
  accessibility, and so on. Every NFR carries a measurable target.

## Labels

| Label | Meaning |
| --- | --- |
| `prd` | Complete PRD (the parent issue) |
| `epic` | Epic |
| `user-story` | User story |
| `fr` | Issue/comment that settles a functional requirement |
| `nfr` | Issue/comment that settles a non-functional requirement |
| `assumption` | Stated without evidence; must be confirmed |
| `open-question` | Unresolved; the PRD records the default used |
| `ready-for-agent` | Fully specified, safe for an AFK agent to implement |
| `wayfinder:map` | Planning map for an in-flight effort |
| `wayfinder:research` | Research ticket |
| `wayfinder:rea` | Reverse-engineering ticket (REA) |
| `wayfinder:prototype` | Prototype ticket |
| `wayfinder:task` | Manual task ticket |

## Evidence rule

No behavioral claim without a citation: `repo/path:line`, a REA tool result, a URL
with section, or a recorded observation. Anything uncited is an assumption and is
labelled as one.
