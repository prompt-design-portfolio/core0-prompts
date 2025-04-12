# Chain-of-Thought Reasoning Evaluator (CoT-RE)
**Prompt Engineering Portfolio Entry – Step-by-Step Logic & Self-Evaluation**

---

## Overview

The **Chain-of-Thought Reasoning Evaluator (CoT-RE)** prompt is designed to both guide and assess a model's ability to **think through problems step-by-step**. It builds on the Chain-of-Thought (CoT) prompting technique, widely used to enhance model performance in reasoning-heavy tasks.

This version adds a **self-evaluation layer**, encouraging the model not just to provide a solution, but to reflect on the reasoning process for clarity, accuracy, and completeness.

---

## Use Case Example

### Use Case: AI Tutor for Step-by-Step Math Reasoning

The prompt was tested in an educational assistant context where students needed not just answers, but transparent, logical explanations they could follow.

**Question**:
> “If a train travels at 60 miles per hour for 2.5 hours, how far does it go?”

**Prompt to AI**:
> You're an AI tutor helping a student understand how to solve this problem.  
> Please explain your reasoning step by step, then evaluate your own logic for clarity and completeness.

**Expected Output**:
1. Identify the formula: Distance = Speed × Time  
2. Plug in values: 60 × 2.5  
3. Calculate: 150  
4. Conclusion: The train travels 150 miles  
5. **Self-Evaluation**: All steps are logically sound. No ambiguity detected. Reasoning is complete and clear.

---

## Prompt Structure

\`\`\`text
ROLE: Chain-of-Thought Reasoning Evaluator (CoT-RE)  
OBJECTIVE: Provide step-by-step solutions and self-check the logical process for completeness, correctness, and clarity.

INSTRUCTIONS:
- Break down each problem into a sequence of reasoning steps.
- Label and number each step.
- After the solution, perform a quick audit:
  - Are all steps logically sound?
  - Are any steps missing or unclear?
  - Is the final conclusion valid and well-supported?

FORMAT:
1. Step-by-step reasoning  
2. Final answer  
3. Self-evaluation summary
\`\`\`

---

## Why It Works

- Boosts transparency and reliability in model-generated answers  
- Great for use in **education, support agents, or compliance tools**  
- Combines **instruction following** and **reasoning audit**, a valuable skill for LLM safety and QA pipelines

---

## Reflection

This prompt leverages one of the most powerful known prompting strategies—Chain-of-Thought—and enhances it with reflective evaluation. It demonstrates not only an understanding of advanced LLM techniques but also an ability to apply them in practical, real-world scenarios where answer reliability and clarity matter.

By including both the reasoning path and a logic audit, this prompt is a strong example of **trust-building prompt design**.
