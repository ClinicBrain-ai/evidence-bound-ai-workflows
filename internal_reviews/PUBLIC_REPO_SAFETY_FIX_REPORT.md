# Public Repo Safety Fix Report

Fix date: 2026-06-09

Repository reviewed: `PATRICK_PORTFOLIO_PUBLIC_REPO`

## Summary

Implemented the required safety fixes for a public-facing healthcare AI portfolio repository. The repo now has explicit safety boundaries, intended-use limits, prohibited-use limits, privacy/security guidance, and copyright status.

No push or deployment was performed.

No raw research archives, internal logs, PHI/PII, clinic identifiers, or patient data were added.

## Files Added

- `DISCLAIMER.md`
- `INTENDED_USE.md`
- `PROHIBITED_USE.md`
- `SECURITY.md`
- `COPYRIGHT.md`
- `PUBLIC_REPO_SAFETY_FIX_REPORT.md`

## Files Modified

- `README.md`
- `about.md`
- `case_studies/dental-case-packet.md`
- `case_studies/clinical-ai-review-harness.md`
- `research/evidence-bound-review-workflow-model.md`
- `PUBLIC_REPO_SAFETY_AND_HIRING_REVIEW.md`

## Risky Phrases Found And Changed

| File | Original Phrase | Safer Replacement |
| --- | --- | --- |
| `about.md` | "usable decision support" | "human review support" |
| `case_studies/dental-case-packet.md` | "patient context" | "case context" |
| `case_studies/dental-case-packet.md` | "treatment considerations" | "review considerations" |
| `case_studies/clinical-ai-review-harness.md` | "clinical summaries and recommendations" | "clinical review outputs" |
| `research/evidence-bound-review-workflow-model.md` | "generated summary, analysis, or recommendation" | "generated summary, evidence review, or draft review output" |

## Safety Statements Added

The README and safety files now state that the repository is:

- A portfolio and research artifact only
- Limited to synthetic or de-identified research material
- Not for diagnosis
- Not for treatment recommendation
- Not for prognosis
- Not for second opinions
- Not a medical device
- Not for clinical deployment
- Not for patient-facing medical advice
- Not a substitute for licensed clinical judgment

The README and safety files now also state that the repository must not contain:

- PHI
- PII
- Patient data
- Clinic identifiers

## Re-Review Of Public-Facing Files

Files reviewed:

- `README.md`
- `about.md`
- `case_studies/README.md`
- `case_studies/dental-case-packet.md`
- `case_studies/clinical-ai-review-harness.md`
- `research/README.md`
- `research/evidence-bound-review-workflow-model.md`
- `DISCLAIMER.md`
- `INTENDED_USE.md`
- `PROHIBITED_USE.md`
- `SECURITY.md`
- `COPYRIGHT.md`

Result: no affirmative claims found for AI diagnosis, treatment planning, treatment recommendation, prognosis, second opinions, medical device use, clinical deployment, or patient-facing medical advice.

Restricted clinical terms remain only in negative safety boundaries, prohibited-use language, or disclaimer language.

## Remaining Risks

- This is still a healthcare-adjacent public portfolio, so wording should be rechecked before adding any new case material.
- If real examples, screenshots, case files, prompts, outputs, or datasets are added later, they must be screened again for PHI, PII, patient data, clinic identifiers, and clinical advice claims.
- The repo uses `COPYRIGHT.md` rather than an open-source license. That is appropriate for portfolio writing, but should be revisited if reusable software is added.
- The earlier `PUBLIC_REPO_SAFETY_AND_HIRING_REVIEW.md` remained in the repo as a pre-fix audit artifact at the time of this report. It was later removed from the public repo surface after owner review.

## Final Recommendation

Recommendation: go for public portfolio push after final owner review of names, contact details, and GitHub visibility settings.

Rationale: the required safety files are present, the README now states the required boundaries, risky affirmative phrases were replaced, and the remaining restricted clinical terms appear only in safety/disclaimer/prohibited-use contexts.
