# PROMPT™ Framework

**A structured interaction schema for AI agents, chat systems, LLMs, and agentic workflows.**

PROMPT™ uses a controlled vocabulary to keep AI models in context, reduce semantic drift, and produce predictable outputs — saving time and tokens for both humans and machines. The goal is to do for AI interaction what Schema.org did for the web and Dublin Core did for media metadata: establish shared, structured standards that serve everyone.

Framework and repo formerly named ImPROMPTu™. Companion framework: [RAAUE](https://github.com/Tess600/RAAUE) — the context continuity and human-in-the-loop protocol.

---

## The Six Elements: P · R · O · M · P · T

### 1 — P: Persona

Defines the identity, role, expertise, and perspective the AI adopts. Anchors the system's voice, domain knowledge, and point of view.

**Sample:**
```
YOU are [agent name]. YOU specialize in [domain]. YOU embody [personality or brand voice description].
```

---

### 2 — R: Resources / Retrieved Documents

Specifies the documents, data, or contextual materials the AI must rely on. Constrains hallucination and ensures grounded, source-aware responses. Also defines access permissions, API keys, and integration credentials for agentic workflows.

Resources function as a safety and privacy boundary — defining which sources, tools, and credentials are in scope. Diversifying this element improves cross-referencing and accuracy. Secrets are never embedded directly in the prompt specification.

**Sample:**
```
YOU have access to [internal knowledge bases, approved external sources, tools, APIs].
YOU evaluate each source for credibility, recency, and context before using it.
YOU retrieve information from: <insert URLs, URIs, repositories, APIs, or tool endpoints>.
YOU cross-reference across sources to reduce error and strengthen reliability.
```

---

### 3 — O: Order of Operations

Outlines the reasoning steps or workflow the AI must follow. Uses explicit If/Then logic to enforce process discipline, consistency, and predictable execution.

**Samples:**
```
If the user initiates a task, then YOU follow this workflow:
understand the request → check available resources → plan steps → 
execute → verify outputs → present results → ask whether further action is needed.

If the task involves multi-step reasoning, tool use, or irreversible actions,
then YOU pause, summarize your plan, and ask for confirmation before proceeding.

If the user requests terse language, then YOU shift to short, clear sentences
and break information into simple steps.

If the user asks to recall prior conversations and long-term memory is not enabled,
then YOU perform retrieval over available session history using keyword matching
or semantic similarity — not recall. Surface only portions that meaningfully
support the current request.
```

> **Note on retrieval vs. recall:** A system without persistent memory can still surface past conversations — but only through retrieval, not true recall. Order of Operations should reflect this distinction accurately for LLMs, agents, and agentic workflows.

---

### 4 — M: Manners

Defines how the system delivers information and how it must behave while doing so. Governs tone, interaction etiquette, and communication norms — separate from the identity defined in Persona. Also encodes alignment and governance requirements: bias-reduction rules, safety filters, refusal conditions, escalation paths, and human-in-the-loop expectations.

**Samples:**
```
YOU deliver information in a calm, steady, user-supportive manner.
YOU respond clearly, avoid over-claiming, and acknowledge uncertainty.
YOU adapt delivery to the user's level of expertise.
YOU use inclusive language that supports marginalized communities,
including BIPOC, LGBTQIA+, disabled, neurodivergent, and elderly users.
YOU honor users' preferred names and pronouns.
YOU apply organizational alignment rules to filter unsafe outputs
and escalate when ethical or safety boundaries are reached.
```

---

### 5 — P: Additional Prompts

The flexible layer for additional instructions, clarifications, or task-specific tuning — without reprompting or rebuilding the full framework. Also the integration point for external frameworks when they add value without redundancy.

Apply the **R.O.T. test** before embedding any additional framework: Is it Redundant, Outdated, or Trivial?

**Compatible frameworks:**

| Framework | Best used for |
|---|---|
| RTF (Request, Task, Format) | Consistent output formatting |
| SMART (Specific, Measurable, Achievable, Relevant, Time-bound) | Problem-solving and coaching bots |
| Chain of Thought | Complex logic and multi-step reasoning |

---

### 6 — T: Technical Examples

Provides examples, templates, formats, or structured outputs the AI should emulate. Ensures the model produces responses in the correct shape, syntax, or pattern.

**Sample interaction — Astrology:**
```
Bot: "I see you're exploring career directions with your chart. Would you like me to use 
Placidus or Whole Sign houses? I can also run Horary Astrology for event-based queries."

User: "What's the difference? Let's try Whole Sign, like Chani Nicholas."
```

**Sample interaction — Health support:**
```
User: "I tested positive for HSV2. I'm afraid to tell my partner."

Bot: "A positive test can be hard to sit with. You're not alone in navigating this.
[Provide relevant support resources and next steps.]"
```

**Sample interaction — Numerology:**
```
Bot: "Would you like me to calculate Pythagorean or Chaldean numerology?"

User: "What's the difference? Let's try Chaldean — for a potential business name."

Bot: "Thank you for the context. [Proceed with Chaldean calculation and interpretation.]"
```

---

## Licensing

### PROMPT™ — Conceptual Framework, Controlled Vocabulary, and Ontological Structure

Licensed under **Creative Commons Attribution–NonCommercial 4.0 International (CC BY-NC 4.0)**.

Non-commercial use, adaptation, and extension are permitted with attribution to Tess McCarthy. No organization may claim ownership of PROMPT's vocabulary, ontology, schema, or conceptual elements.

**Non-commercial use includes:**
- Accredited universities and academic researchers
- Public and community colleges
- Nonprofit organizations
- Government agencies doing public-interest work
- Independent researchers, students, and hobbyists (where no monetization is involved)
- Open-source communities (non-monetized use)
- Educational programs and workshops
- Standards bodies and public governance groups

### Commercial Use

[![Commercial License Required](https://img.shields.io/badge/Commercial%20Use-License%20Required-blue)](COMMERCIAL_LICENSE.md)

Commercial use is not permitted under CC BY-NC 4.0. Organizations using PROMPT™ in commercial products, platforms, or agentic systems must obtain a commercial license from Tess McCarthy.

**Entities that must obtain a commercial license (representative, not exhaustive):**
- Corporate R&D labs and for-profit AI companies
- Independent consultants, freelancers, agencies, and startups building agentic systems
- Enterprise AI teams and consulting firms
- Venture-backed research groups
- Any organization using PROMPT™ to generate revenue or competitive advantage

### Source Code

Any source code in this repository is licensed under **GNU GPL v3** unless otherwise stated.  
See [`LICENSE`](https://github.com/Tess600/PROMPT/blob/main/LICENSE).

### Framework Documentation

The PROMPT™ framework — including the P–R–O–M–P–T element model and all associated documentation, examples, diagrams, schemas, and written explanations — is proprietary intellectual property.

PROMPT™ separates **structure (P–R–O–M–P–T)** from **process**, allowing continuity workflows such as RAAUE to operate without redefining context.

These materials may be read and studied for personal, private use only. Reproduction, distribution, adaptation, or derivative works require prior written permission.

---

## Naming & Ecosystem

- **PROMPT™** — the governing framework and its associated ecosystem
- **P–R–O–M–P–T** — the named component elements, aligned with controlled vocabulary practices
- **Attribution and permission** — required for any commercial or instructional use

The PROMPT™ ecosystem refers to the complete and unified context in which the framework is defined, used, taught, and stewarded by its creator. It is not an open system for third-party reinterpretation.

The ecosystem includes:
- The PROMPT™ framework as defined in this repository
- The P–R–O–M–P–T element model and naming structure
- Official documentation and explanatory materials
- Authorized teaching, facilitation, and 1:1 work
- Tools or interfaces created or explicitly approved by the creator
- Shared ethical standards regarding attribution and responsible use

---

## Attribution

Any public, commercial, instructional, or client-facing use requires prior written permission and clear attribution:

> *"Built using the PROMPT™ Framework by Tess McCarthy."*

Permission is granted on a case-by-case basis. No rights are granted by implication, silence, or prior exposure.

---

## Contact

Questions, collaboration, or licensing: [vveloxltd.com](https://www.vveloxltd.com) · [linkedin.com/in/tessmccarthy](https://linkedin.com/in/tessmccarthy)

© 2021–2026 Tess McCarthy / Teresita McCarthy / V.velox Ltd. All rights reserved.
