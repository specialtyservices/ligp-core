# LLM Interaction Governance Protocol (LIGP)

*A user-side protocol for governable, inspectable, and repeatable interaction with Large Language Models.*

---

## Status

- **Version:** v1.0  
- **Maturity:** Stable — initial public normative release  
- **Classification:** Interaction-layer protocol  
- **License:** CC BY-SA 4.0 (see ATTRIBUTION.md)  
- **Maintenance:** Active  
- **Audience:** Professional, regulated, and authorship-sensitive use  

---

## What This Repository Is

This repository contains the **authoritative reference documentation** of the **LLM Interaction Governance Protocol (LIGP)**.

LIGP is a formal interaction protocol that governs how a user interacts with a Large Language Model (LLM), with explicit separation between:

- persistent personal context (where enabled),
- session-local behavioral inference,
- explicit user instruction.

The protocol operates entirely at the **human–LLM interaction layer** and does **not** require access to model internals, training data, or system policies.

This repository is intended to function as **standard infrastructure**, not as editorial content, prompt collections, or a commercial product.

---

## What This Repository Is Not

- Not prompt engineering  
- Not a model alignment technique  
- Not a memory optimization hack  
- Not an AI safety or control system  
- Not certification, compliance assurance, or legal advice  
- Not a proprietary or closed framework  

LIGP governs **interaction behavior only**.

---

## Scope

### In Scope

- Inspection and governance of persistent personal context (where available)
- Visibility into session-local behavioral inference
- Explicit, stateless reconstruction of interaction behavior via instruction
- Deterministic interaction continuity without reliance on memory or profiling

### Out of Scope

- Model training or fine-tuning
- Dataset provenance
- Internal parameters or embeddings
- System-level safety policy enforcement
- Infrastructure security

---

## Core Components

LIGP consists of three **orthogonal protocol components**:

### 1. Persistent Context Audit

A governance mechanism to inspect, verify, correct, or delete any user-specific information treated as long-term personal context.

### 2. Session-Local Behavioral Transparency

A reflective disclosure that makes session-local adaptation visible without implying persistence, profiling, or storage.

### 3. Stateless Behavioral Instruction Block

A reusable, explicit declaration of interaction constraints provided at session start, enabling deterministic behavior reconstruction across sessions.

These components are **sequential, complementary, and non-interchangeable**.

---

## Documentation

### Core Specification

- **Whitepaper**  
  `docs/whitepaper/ligp_whitepaper.md`  
  Authoritative conceptual and architectural description of LIGP.

### Governance & Policy

- **Regulatory Briefing Note**  
  `docs/regulatory/ligp_regulatory_briefing.md`  
  Policy-facing overview for regulators, compliance leaders, and governance bodies.

- **Enterprise Governance Mapping**  
  `docs/enterprise/ligp_enterprise_governance_mapping.md`  
  Alignment of LIGP with ISO, EU AI Act, OECD, and enterprise governance frameworks.

### Licensing & Reuse

- **Licensing & Attribution**  
  `ATTRIBUTION.md`  
  Conditions for reuse, attribution, and derivative work.

---

## Repository Structure

.
├── README.md

├── LICENSE

├── ATTRIBUTION.md

└── docs

├── whitepaper

│   └── ligp_whitepaper.md

├── regulatory

│   └── ligp_regulatory_briefing.md

├── enterprise

│   └── ligp_enterprise_governance_mapping.md

└── licensing

└── ligp_licensing_and_attribution.md

---

## Design Intent

LIGP does not attempt to make AI systems fully transparent.

It makes **interaction governable**.

By separating storage, inference, and instruction, LIGP enables auditability, repeatability, and user-side control without requiring internal access to model implementations.

---

## Attribution

Any reuse or adaptation of LIGP **must comply** with the attribution and licensing terms defined in `ATTRIBUTION.md`.
