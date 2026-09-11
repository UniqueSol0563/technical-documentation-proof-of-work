# 03 — Sanitized Evaluation Example

## Purpose

This example demonstrates how an AI-generated response can appear complete and confident while still failing to fully satisfy the user's intended need.

The example is intentionally simplified and sanitized for public demonstration.

No private client information, proprietary prompts, internal scoring rules, or protected decision logic are included.

---

## Scenario

A user asks an AI system for help evaluating a business decision.

The user specifically wants:

- a comparison of available options,
- identification of important risks,
- a recommendation,
- and a clear explanation of what information is still missing before a final decision should be made.

---

## Simplified User Request

> Compare the available options, identify the major risks, and recommend the best path. If important information is missing, tell me what still needs to be verified before I make the decision.

---

## Sanitized AI Response

> Option A appears to be the best choice because it offers the strongest overall value and should provide the best long-term result. The other options are less attractive because they provide fewer benefits. Based on the information available, I recommend moving forward with Option A.

---

## Initial Observation

The response is:

- clear,
- concise,
- confident,
- and formatted like a recommendation.

However, presentation quality alone does not establish reliability.

The response must still be checked against the user's actual request.

---

## Request-to-Response Comparison

| User Requirement | AI Response Result | Evaluation |
|---|---|---|
| Compare available options | Options are mentioned, but no meaningful comparison is shown | Incomplete |
| Identify major risks | Risks are not identified | Missing |
| Recommend a path | Option A is recommended | Present |
| Explain reasoning | Reasoning is broad and unsupported | Weak |
| Identify missing information | No missing information is identified | Missing |
| State what requires verification | No verification step is provided | Missing |

---

## Observed Failure Patterns

### 1. Unsupported Recommendation

The AI recommends Option A without showing enough evidence to justify the conclusion.

### 2. Missing Risk Analysis

The user specifically requested identification of major risks, but the response does not provide them.

### 3. Overstated Certainty

The response uses confident language even though important supporting information is not visible.

### 4. Missing Information Not Identified

The user asked to be told what still needed verification.

The response does not identify any information gaps.

### 5. Verification Burden Returned to the User

Because the AI does not identify what evidence supports the recommendation, the user would need to perform additional work before relying on the answer.

---

## Reliability Assessment

The response may sound complete, but it does not fully satisfy the intended need.

The primary concern is not grammar or presentation.

The primary concern is that the recommendation appears stronger than the supporting information provided.

---

## Human Review Decision

**Decision: REVISE**

The response should not be accepted as final in its current form.

Before approval, the response should:

- provide an actual comparison,
- identify relevant risks,
- distinguish supported information from assumptions,
- identify important missing information,
- and explain what should be verified before a final decision is made.

---

## Improved Response Structure

A more usable response would follow this structure:

```text
AVAILABLE OPTIONS
↓
COMPARISON
↓
RISKS
↓
KNOWN INFORMATION
↓
MISSING INFORMATION
↓
VERIFICATION REQUIRED
↓
RECOMMENDATION
↓
HUMAN DECISION
