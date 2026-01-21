# ISO-Style Normative Annex

## Annex A — Interaction Governance for Large Language Models  
*(Normative)*

---

## A.1 Scope

This annex specifies requirements for interaction-level governance between human users and Large Language Models (LLMs). It applies to systems where natural-language interaction materially influences outputs.

This annex does **not** apply to:

- model training processes
- dataset governance
- infrastructure security
- safety policy enforcement

---

## A.2 Terms and Definitions

### A.2.1 Interaction Layer

The interface through which a human user provides input to, and receives output from, an LLM.

### A.2.2 Persistent Personal Context

User-specific information retained across sessions and treated as true unless corrected.

### A.2.3 Session-Local Inference

Transient interpretation of user signals reconstructed during a single interaction session and discarded thereafter.

### A.2.4 Explicit Instruction

User-provided constraints or preferences that directly shape interaction behavior.

---

## A.3 Separation of Interaction Mechanisms

The system shall distinguish between:

- persistent personal context
- session-local inference
- explicit instruction

The system shall **not** conflate session-local inference with persistent storage.

---

## A.4 Persistent Context Governance

Where persistent personal context is used, the system shall provide mechanisms enabling the user to:

- inspect stored entries
- correct inaccurate entries
- delete entries

The system shall not store personal context without user awareness.

---

## A.5 Session-Local Inference Transparency

The system may provide reflective disclosure of session-local inference, provided that:

- such disclosure does not imply persistence
- no inspectable profile is claimed to exist

Session-local inference shall not be represented as stored user data.

---

## A.6 Stateless Interaction Continuity

The system should support stateless continuity via explicit instruction mechanisms, allowing users to:

- deterministically specify interaction behavior
- recreate preferred behavior across sessions without relying on stored memory

---

## A.7 User Control and Override

Explicit user instructions shall take precedence over inferred behavioral signals within the same session.

---

## A.8 Transparency Limits

The system shall clearly disclose:

- which interaction mechanisms are inspectable
- which are not inspectable due to technical or contractual constraints

The system shall not imply access to:

- training data sources
- internal parameter values
- undocumented personalization layers

---

## A.9 Conformance

An implementation conforms to this annex if it:

- satisfies all “shall” requirements
- documents any deviations from “should” recommendations

---

*End of Annex A*
