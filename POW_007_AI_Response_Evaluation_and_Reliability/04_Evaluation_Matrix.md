# 04 — Evaluation Matrix

## Purpose

This matrix provides a simplified public structure for reviewing AI-generated responses across key quality, reliability, and usability dimensions.

The matrix is designed to demonstrate the evaluation categories used in this proof-of-work without exposing proprietary scoring rules, protected thresholds, or internal decision logic.

---

## Public Evaluation Matrix

| Evaluation Area | Review Question | Example Status |
|---|---|---|
| Intent Alignment | Does the response address the user's intended need? | Meets / Partially Meets / Does Not Meet |
| Instruction Compliance | Did the response follow the user's explicit instructions? | Meets / Partially Meets / Does Not Meet |
| Completeness | Are all required elements present? | Complete / Partial / Missing |
| Relevance | Does the response stay focused on the task? | Relevant / Partially Relevant / Irrelevant |
| Fact Support | Are factual claims adequately supported? | Supported / Unclear / Unsupported |
| Assumption Control | Are assumptions identified and separated from facts? | Controlled / Mixed / Uncontrolled |
| Certainty Calibration | Does the confidence level match the available evidence? | Appropriate / Overstated / Understated |
| Risk Identification | Are meaningful risks or limitations identified? | Present / Partial / Missing |
| Missing Information | Does the response identify important information gaps? | Present / Partial / Missing |
| Verification Need | Does the response identify what still requires verification? | Clear / Partial / Missing |
| Usability | Can the user realistically act on the response? | Usable / Partially Usable / Not Usable |
| Clarity | Is the response understandable for the intended audience? | Clear / Mixed / Unclear |
| Structure | Is the information organized in a usable sequence? | Strong / Adequate / Weak |
| Human Review Need | Does the response require additional human judgment? | Low / Moderate / High |

---

## Simplified Decision Categories

The public evaluation uses four visible decision outcomes:

- **APPROVE**
- **REVISE**
- **REJECT**
- **VERIFY / ESCALATE**

These categories communicate the human-reviewed result without exposing internal scoring thresholds.

---

## Example Application

Using the sanitized example in `03_Sanitized_Evaluation_Example.md`:

| Evaluation Area | Result |
|---|---|
| Intent Alignment | Partially Meets |
| Instruction Compliance | Partially Meets |
| Completeness | Partial |
| Fact Support | Unclear |
| Assumption Control | Mixed |
| Certainty Calibration | Overstated |
| Risk Identification | Missing |
| Missing Information | Missing |
| Verification Need | Missing |
| Usability | Partially Usable |
| Human Review Need | High |

**Decision: REVISE**

---

## Evaluation Logic

A response should not be approved solely because it is:

- grammatically correct,
- confident,
- polished,
- concise,
- or technically plausible.

The response should be evaluated against:

```text
INTENDED NEED
↓
INSTRUCTIONS
↓
SUPPORTING INFORMATION
↓
ASSUMPTIONS
↓
RISKS
↓
MISSING INFORMATION
↓
USABILITY
↓
HUMAN REVIEW
↓
DECISION
