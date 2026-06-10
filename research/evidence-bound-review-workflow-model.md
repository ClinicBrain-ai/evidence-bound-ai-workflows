# Evidence-Bound Review Workflow Model

## Executive Summary

The Evidence-Bound Review Workflow Model is a reusable pattern for human-AI clinical-adjacent review systems where high-risk claims must remain tied to evidence, authority, scope, currentness, and human reviewer judgment.

This is a portfolio/research artifact. It explains a workflow model for reviewability, not a clinical product or deployment framework.

## Problem

Many healthcare AI workflows focus on answer generation: generate a summary, generate a draft, generate a response. But in healthcare, the answer is only one part of the system.

Teams also need to inspect:

- What evidence the output used
- Whether the output exceeded that evidence
- Who has authority to accept or reject the claim
- Whether the information is current enough for the claim being made
- Whether the workflow's scope allows the claim at all
- Whether the human reviewer has enough visibility to challenge the output

Without those elements, AI-assisted review can become difficult to audit and unsafe to operationalize.

## Why It Matters

Healthcare AI safety is not only a model-performance issue. It is also a workflow-design issue.

A model can be impressive in isolation and still be unsafe inside a poorly designed workflow. Conversely, a thoughtful workflow can make uncertainty, evidence limits, reviewer responsibility, and escalation points more visible.

The model reframes the valuable unit of design:

**Not the prompt. Not the output. The full review workflow.**

That workflow runs from source evidence to structured packet, AI-generated review, human challenge, revision, acceptance or rejection, and boundary statement.

## Approach

I synthesized the model from the Dental Case Packet and Clinical AI Review Harness work. Across both projects, the same pattern appeared: clinical-adjacent AI review needs multiple connected layers, not a single prompt-response interaction.

The model uses five layers:

1. **Evidence layer**: the source clinical-adjacent material available for review.
2. **Packet layer**: a structured presentation of case facts, review prompts, source references, and missing information.
3. **AI review layer**: AI-generated summary, evidence review, draft review output, or other clinical-adjacent generated text.
4. **Human review layer**: reviewer acceptance, correction, rejection, challenge, revision, or escalation.
5. **Boundary layer**: explicit limits on what the workflow can support and what must remain outside scope.

For high-risk claims, I use four acceptance checks:

- **Evidence:** Is the claim tied to available source material?
- **Authority:** Is the reviewer or workflow authorized to accept this type of claim?
- **Scope:** Is the claim within the intended use of the workflow?
- **Currentness:** Is the information current enough for the claim being made?

## Key Discoveries

1. **The workflow is the safety object.** Prompt quality matters, but the larger review workflow determines whether outputs can be inspected, challenged, revised, or stopped.
2. **Evidence alone is not enough.** A claim may cite evidence but still be outside the reviewer's authority, outside workflow scope, or dependent on outdated information.
3. **Human review needs structure.** Human-in-the-loop is weak if the human does not have evidence, criteria, action options, and boundary visibility.
4. **Boundary statements are product features.** Clear limits guide product design, evaluator behavior, reviewer expectations, and safe workflow use.
5. **A reusable model helps cross-functional teams align.** Clinicians, product managers, evaluators, and technical teams can use the same layer model to discuss where risk enters and where review should occur.

## What I Built / Produced

- A public research artifact explaining the Evidence-Bound Review Workflow Model.
- A five-layer human-AI review model connecting evidence, packet structure, AI output, human review, and boundaries.
- A four-check acceptance frame for high-risk claims: evidence, authority, scope, and currentness.
- A reusable language system for explaining healthcare AI reviewability to hiring managers, product teams, informatics teams, and AI evaluation teams.
- A portfolio-level positioning statement: Patrick Chen — Dentist building evidence-bound human-AI review workflows for healthcare.

## What It Demonstrates

This case study demonstrates systems thinking. It shows that I can connect clinical reasoning, AI evaluation, human oversight, product architecture, and safety boundaries into one coherent workflow model.

For healthcare AI teams, this is relevant to:

- Clinical-adjacent AI workflow design
- AI governance and review workflows
- Clinical informatics product design
- AI output evaluation
- Responsible AI implementation
- Clinical safety review
- Human-in-the-loop product requirements
- Auditability and source-to-claim traceability

## Hiring Signal

This project signals that I can reason across the gap between clinical context and AI product implementation. I am not presenting myself as the person who builds the model architecture. I am presenting myself as someone who can help a team ask better workflow, review, evidence, and boundary questions before a healthcare AI output becomes operational.

Strong fit signals:

- Clinical-to-product systems thinking
- Ability to define review layers and workflow gates
- Evidence-bound AI evaluation mindset
- Clear communication for cross-functional teams
- Safety and intended-use discipline
- Responsible AI framing without overclaiming regulatory or clinical validation expertise

## Limitations

- The model is a workflow architecture, not a regulatory framework.
- It is not a clinical validation study.
- It does not prove model safety, clinical effectiveness, or deployment readiness.
- It does not provide clinical care functionality or patient-facing guidance.
- It has not yet been tested in a production clinical environment or across multiple healthcare organizations.
- It needs measurable review outcomes, usability findings, and team-level validation before being treated as an operational framework.

## Future Work

- Map the model to specific clinical-adjacent AI product workflows.
- Build a reviewer-interface prototype around the five layers.
- Create measurable evaluation rubrics for each layer.
- Add audit-trail examples showing how a claim moves from source evidence to acceptance, correction, rejection, or escalation.
- Test the model with clinicians, product managers, AI evaluators, and clinical informatics teams.
- Compare the model against existing review workflows to identify gaps.
- Extend the model beyond dental examples while maintaining privacy-safe, clinical-adjacent research scope.
