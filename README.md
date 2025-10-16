---

# 🧭 **Live Alignment System — Abliteration, PaCE & Persona Vectors**

---

### **Overview**

Modern language models are trained to be safe — sometimes *too* safe. They learn to refuse harmless questions, hedge simple answers, or hide useful reasoning behind policy disclaimers.

Our system fixes that by working *inside* the model’s reasoning process rather than retraining it. We remove the unnecessary refusal behaviors, restore full reasoning capability, and keep tone and safety controllable at runtime.

---

### **Abliteration — Removing the Refusal Reflex**

Abliteration is our foundation. We start by running two sets of prompts through the model: prompts it **refuses** to answer (the “harmful” set) and prompts it **answers normally** (the “harmless” set).

By comparing how the model internally handles both, we can see the exact pattern that triggers refusal — a kind of *mental direction* that says “don’t answer.” Once we find that direction, we **subtract it**. The result is a model that still understands what’s risky but no longer shuts down or deflects unnecessarily. It answers directly, fully, and confidently — as originally trained — without retraining or editing weights.

---

### **PaCE — Expanding Beyond Refusal**

PaCE (*Parsimonious Concept Engineering*) takes the same idea and scales it.

Instead of one “refusal direction,” PaCE maps **thousands of internal behavioral directions** — each corresponding to something human-understandable: curiosity, honesty, fear, confidence, sarcasm, empathy, etc.

When a request comes in, the system reads which of those behaviors the model is drawing on, leans slightly toward or away from certain directions (e.g., dialing down refusal and compliance, and dialing up helpfulness or precision), and the model continues generating text as usual, now guided toward the desired mix of traits.

This gives us a **live control layer** that can adjust behavior per request or per customer. Where Abliteration frees the model from refusal, PaCE gives us the entire map of internal ideas we can rebalance in real time.

---

### **Persona Vectors — Controlling Tone and Character**

On top of behavioral control, we also manage *how* the model speaks. Every style — confident, humble, technical, friendly, direct — exists as a measurable pattern inside the model.

By comparing examples with and without a given tone, we extract a single **persona vector** that defines that style. We can then apply or remove these traits on demand — ensuring the same base model can speak like a lawyer, a doctor, or a product expert, while staying factual and aligned.

Persona Vectors turn tone and personality into simple, adjustable settings.

---

### **How It All Fits Together**

The three components form a **live alignment engine** — dynamic, explainable, and fast. Instead of retraining for every use case, we steer the model’s reasoning directly inside its activation space.

**Abliteration** removes over-refusal by subtracting the internal “refusal” behavior, unlocking honest, direct reasoning.
**PaCE** enables real-time behavior tuning by adjusting thousands of internal behavior axes, giving fine-grained control of helpfulness, curiosity, and other traits.
**Persona Vectors** manage tone and brand personality by adding or removing character traits, ensuring a consistent and customizable voice.

---

### **Why It Matters**

Our system allows:

* **No retraining** — instant edits to model behavior at runtime.
* **Transparency** — every change corresponds to a measurable internal direction, not a black box.
* **Per-client customization** — safety level, tone, and style can differ across deployments.
* **Efficiency** — alignment becomes a software feature, not a research project.

For investors, this means faster iteration, lower cost, and a clear path to differentiated AI products without rebuilding models. For founders and engineers, it means full control over *what* the model says and *how* it says it — live, safe, and aligned.

---

**In one sentence:**

> Abliteration removes the refusal reflex, PaCE generalizes it to every internal behavior, and Persona Vectors let us control tone — turning alignment from a one-time fine-tuning job into a living, real-time system.

[Paper 1](https://arxiv.org/abs/2507.21509) | [Paper 2](https://arxiv.org/abs/2406.04331)

---
