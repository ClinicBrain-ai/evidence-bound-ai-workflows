# Evidence-Bound AI Workflows

Patrick Chen — Dentist building evidence-bound human-AI review workflows for healthcare.

This repository presents three public-facing portfolio artifacts for healthcare AI, clinical informatics, AI evaluation, and clinical product teams. It is designed for 30-second comprehension: each page explains the problem, the artifact, the architecture, the boundaries, and the hiring signal.

## Safety Notice

This repository is a portfolio and research artifact only. It is limited to synthetic or de-identified research material.

This repository does not contain PHI, PII, patient data, or clinic identifiers.

This repository is not for diagnosis, treatment recommendation, prognosis, second opinions, medical device use, clinical deployment, or patient-facing medical advice. It is not a substitute for licensed clinical judgment.

## Portfolio Focus

The work centers on a practical question:

How can clinical AI workflows make reasoning, evidence use, reviewer judgment, and model boundaries visible enough to be inspected?

## Included Work

| Artifact | What It Shows | Best Audience |
| --- | --- | --- |
| [Dental Case Packet](case_studies/dental-case-packet.md) | Structures synthetic or de-identified clinical-adjacent case material before human review | Clinical AI product teams, clinical informatics teams |
| [Clinical AI Review Harness](case_studies/clinical-ai-review-harness.md) | Evaluates AI-generated clinical-adjacent outputs against source evidence and reviewer criteria | AI evaluation teams, healthcare AI hiring managers |
| [Evidence-Bound Review Workflow Model](research/evidence-bound-review-workflow-model.md) | Connects evidence, AI output, human review, and workflow boundaries into a reusable model | Clinical AI product teams, AI evaluation teams |

## Companion Repositories

| Repository | Role In Portfolio | Boundary |
| --- | --- | --- |
| [Evidence-Bound Clinical Review Toolkit](https://github.com/ClinicBrain-ai/evidence-bound-clinical-review-toolkit) | Converts AI-generated healthcare-adjacent outputs into evidence-linked, human-reviewable Clinical Review Packets | Review infrastructure only; not clinical use |
| [Evidence-Bound AI Evaluation Harness](https://github.com/ClinicBrain-ai/evidence-bound-ai-evaluation-harness) | Evaluates AI-generated healthcare-adjacent outputs for unsupported claims, missing context, uncertainty gaps, source conflicts, scope-boundary issues, and human-review routing | Reviewability and evidence-alignment only; not clinical correctness validation |

## Repository Structure

```text
PATRICK_PORTFOLIO_PUBLIC_REPO/
  README.md
  about.md
  DISCLAIMER.md
  INTENDED_USE.md
  PROHIBITED_USE.md
  SECURITY.md
  COPYRIGHT.md
  case_studies/
  research/
```

## What This Repository Does Not Include

This public repo excludes internal materials that are not appropriate for a hiring-facing portfolio:

- Internal discovery logs
- Primitive research drafts
- Protocol iterations
- Counterexample notebooks
- Raw research archives
- Patient data, PHI, PII, and clinic identifiers

## Positioning

This is not a claim to a fixed job title. The public signal is narrower and stronger:

Patrick Chen — Dentist building evidence-bound human-AI review workflows for healthcare.
