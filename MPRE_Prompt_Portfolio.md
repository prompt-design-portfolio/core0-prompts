# Multi-Perspective Reasoning Engine (MPRE)
**Prompt Engineering Portfolio Entry – Simulated Expert Deliberation**

---

## Overview

The **Multi-Perspective Reasoning Engine (MPRE)** is a prompt framework that transforms a language model into a **panel of simulated experts**, each offering a distinct viewpoint on a complex question or problem. Rather than delivering a single answer, the model simulates **multi-agent debate and synthesis**.

This allows the LLM to offer richer, more nuanced insights—perfect for use in decision-making tools, ethical design, product strategy, and knowledge synthesis.

---

## Use Case Example

### Use Case: AI Advisor for Ethical Tech Design

A product team is exploring whether to implement biometric user identification in a public app. They want diverse perspectives to guide a responsible decision.

**Prompted Scenario**:
> “Should biometric user identification be required in a public-facing app?”

**Prompt Behavior**:
The model simulates the following perspectives:
- **Privacy Advocate**
- **Product Manager**
- **Security Engineer**
- **Accessibility Consultant**

**MPRE Output**:
- **Privacy Advocate**: Opposes mandatory biometrics due to consent and surveillance concerns.
- **Product Manager**: Sees benefits in user friction reduction, but flags potential user drop-off.
- **Security Engineer**: Supports it for fraud reduction, but only with encryption safeguards.
- **Accessibility Consultant**: Cautions that biometric systems can exclude disabled users.

**Synthesized Insight**:
> “Biometric ID could enhance security and streamline UX, but mandates risk marginalizing users. A hybrid opt-in model with strong encryption and alternatives for accessibility would balance priorities.”

---

## Prompt Structure

```
ROLE: Multi-Perspective Reasoning Engine (MPRE)  
INSTRUCTIONS:  
Simulate a panel of diverse expert personas. Each responds to the scenario from their domain.  
Then, synthesize a conclusion that reflects the most informed, balanced perspective.

FORMAT:  
- [Persona 1]: [Perspective]  
- [Persona 2]: [Perspective]  
- ...  
- **Synthesis**: [Summary that integrates and evaluates all viewpoints]

SCENARIO: [Insert open-ended question or dilemma]
```

---

## Why It Works

- Encourages **reasoning from multiple worldviews**, not just a single narrative  
- Helps users explore **ethical, technical, and human factors** side-by-side  
- Offers a practical framework for **debate simulation and decision support**

---

## Reflection

This prompt is more than Q&A—it’s a **tool for structured cognitive diversity**. By simulating multi-agent discussion within a single model, it reveals deeper insights and helps users think through complex issues with empathy and rigor.

MPRE is ideal for use in AI co-pilots, policy planning, AI safety research, or any system requiring **considered, multi-dimensional guidance**.
