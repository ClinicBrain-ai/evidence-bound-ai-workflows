# Clinical AI Review Harness

## Executive Summary

The Clinical AI Review Harness is a structured evaluation workflow for reviewing AI-generated clinical outputs against explicit source evidence and reviewer criteria. It helps identify whether an AI response is grounded, overextended, incomplete, or clinically unsafe.

## Problem

Clinical AI outputs can sound coherent while drifting beyond the evidence. Product teams and evaluators need a way to inspect not only the final answer, but also how well the answer stays bound to the case material and the review task.

## Discovery

The harness was developed from repeated review cycles where AI-generated clinical review outputs needed to be checked against source packets. The main discovery was that evaluation needs to capture claim quality, evidence alignment, omissions, uncertainty handling, and revision behavior.

## Architecture

The harness is organized around a repeatable review loop:

- Input case packet
- AI-generated review
- Evidence check
- Claim classification
- Reviewer judgment
- Revision notes
- Boundary assessment

The key design choice is to evaluate the relationship between claims and evidence, not just the surface quality of the generated text.

## Limitations

The harness does not certify clinical correctness by itself. It depends on reviewer expertise, well-formed synthetic or de-identified case packets, and clear evaluation criteria. It is strongest as a review and evaluation scaffold, not as a standalone safety system, diagnostic tool, treatment recommendation tool, second-opinion system, medical device, or patient-facing advice system.

## Future Work

Future versions could include inter-rater reliability tracking, rubric scoring, model comparison views, structured failure taxonomies, and integration with annotation or evaluation tooling.

## Hiring Signal

This project shows practical judgment in clinical AI evaluation: grounding, omission detection, review criteria, human oversight, and workflow design. It is relevant to AI evaluation teams, healthcare AI product teams, and clinical safety review functions.
