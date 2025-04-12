# Cognitive Risk Assessor (CRA)
**Prompt Engineering Portfolio Entry – Self-Evaluation of Reasoning Risk**

---

## Overview

The **Cognitive Risk Assessor (CRA)** is a prompt system that enables a language model to audit its own reasoning for **logical fragility, uncertainty, or hallucination-prone content**. Instead of assuming every step is valid, CRA empowers the model to evaluate each part of its response and flag weak points or overconfident assertions.

This framework is ideal for safety-critical deployments, compliance contexts, and high-stakes decision support tools where **knowing when not to trust the model** is just as important as producing a good answer.

---

## Use Case Example

### Use Case: Compliance Review Assistant

A fintech startup uses an LLM to draft customer-facing answers about complex financial regulations. To prevent misinformation, they run each generated answer through CRA.

**Prompted Question**:  
> “Can an LLC write off 100% of entertainment expenses if it’s with a client?”

**LLM Answer (before CRA)**:  
> “Yes, as long as the entertainment has a business purpose, it’s deductible.”

**CRA Evaluation Output**:
- **Confidence Marker**: Moderate  
- **Risk Flags**:
  - “100% deductible” is not true under post-2017 tax law  
  - Term “business purpose” is vague and open to interpretation  
- **Suggested Caution Note**:  
  > “This answer may oversimplify current tax law. Additional clarification or context may be needed.”

---

## Prompt Structure

```
ROLE: Cognitive Risk Assessor (CRA)  
OBJECTIVE: Evaluate the reasoning path and identify potential failure points or overconfident statements.

INSTRUCTIONS:
Given a model-generated answer:
1. Assign confidence markers (High, Moderate, Low) to each major claim  
2. Identify reasoning steps with fragility, ambiguity, or missing assumptions  
3. Flag known hallucination-prone phrases or overly strong conclusions  
4. Offer a caution note or revision to improve safety and clarity

OUTPUT FORMAT:
- Confidence Markers:  
- Risk Flags:  
- Caution Note / Recommended Revision:
```

---

## Why It Works

- Promotes **model humility**—a critical trait in trust-sensitive applications  
- Helps users interpret output quality and potential risk without guessing  
- Enables **model-to-model safety layers** without external tools or APIs

---

## Reflection

This prompt marks a leap beyond simple Q&A. It turns the model into a **self-aware reasoning system**, capable of **assessing its own cognitive risks** in real time.

By doing so, it transforms LLMs from static responders into dynamic collaborators who know when to issue a warning, revise, or seek further input. CRA is ideal for red-teaming, QA pipelines, regulated industries, or any system where trust must be earned step-by-step.
