# CHVE – Common Human Vulnerabilities & Exposures

> *Humans are unique. Vulnerabilities are shared.*

CHVE (Common Human Vulnerabilities & Exposures) is an open, community-driven catalog of **individual-level cognitive, social, and behavioral vulnerabilities** that can be exploited to influence, manipulate, mislead, or systematically distort human decision-making.

Inspired by the CVE (Common Vulnerabilities and Exposures) system used in cybersecurity, CHVE applies similar rigor and structure to **humans and other probabilistic systems**, including AI models trained on human data.

This project started as a joke.  
It stopped being one when the joke kept working.

---

## Why CHVE exists

Traditional vulnerability models were designed for **deterministic systems**: the same input reliably produces the same output. This assumption works well for classical software, but it breaks down for **probabilistic systems**.

Modern AI systems demonstrably have vulnerabilities as well. Despite their non-deterministic behavior, these vulnerabilities are observable, repeatable in practice, and are already being reported and tracked using adapted security models.

Humans are also probabilistic systems. Individual behavior is shaped by genetics, environment, past experience, and context. However, when observed across populations, humans show **strong behavioral convergence**: under similar conditions, many individuals reliably make similar errors, take similar cognitive shortcuts, and fall prey to similar forms of manipulation.

Attackers do not require certainty. They require **reliable probability at scale**.

CHVE exists to document these *common, exploitable human failure modes*, using a structure inspired by vulnerability tracking in software and AI systems.

---

## What CHVE is

* A **reference catalog**, not a diagnostic or assessment tool
* A catalog of **repeatedly observable vulnerabilities**, independent of whether they are discussed at an individual or population level
* A **threat-modeling abstraction** focused on exploitability rather than explanation or attribution
* A **shared vocabulary** for discussing manipulation, scams, persuasion, logical fallacies, and other exploitable failure modes

Each CHVE entry describes:

- A recurring individual-level human vulnerability
- The conditions under which it emerges
- How it is commonly exploited
- Its typical impact
- Practical mitigations ("human patches")

---

## What CHVE is not

CHVE does **not**:

- Label individuals as "vulnerable"

- Claim universality or determinism

- Assign moral judgment

- Replace psychology, philosophy, or ethics

- Predict individual behavior

CHVEs describe **patterns**, not people.

---

## Deterministic vs probabilistic vulnerabilities

Traditional vulnerability models were largely developed with systems in mind whose behavior is **often deterministic** under controlled conditions. In practice, even software systems can exhibit non-determinism due to configuration, environment, concurrency, or undefined behavior.

CHVE uses a softer distinction, focusing not on strict determinism but on **how exploitation manifests in practice**:

| Domain     | Typical behavior    | Exploit model              |
| ---------- | ------------------- | -------------------------- |
| Software   | Often deterministic | High-reliability execution |
| Humans     | Probabilistic       | Statistical success        |
| AI systems | Probabilistic       | Context-dependent bias     |

CHVE explicitly embraces **probabilistic exploitability**. A vulnerability is considered valid if it can be exploited with *non-trivial, repeatable probability under comparable conditions*.

---

## Scope and applicability

CHVEs apply **exclusively to humans**.

CHVE is explicitly *not* a catalog of AI, animal, organizational, or machine vulnerabilities.

---

## CHVE identifier format

Each vulnerability is assigned a stable identifier:

```
CHVE-YYYY-NNNN
```

Example:

- `CHVE-2026-0001` – Authority Bias

Identifiers are used for reference, discussion, and citation — not severity ranking.

---

## CHVE document structure

Each CHVE is documented as a single Markdown file and typically includes:

- Summary

- Description

- Affected Population

- Applicable Targets (Humans / AI / Hybrid)

- Attack Vectors

- Exploit Examples

- Preconditions

- Impact

- Exploit Reliability (deterministic vs probabilistic)

- Population Convergence

- Mitigations (Human Patches)

- Related CHVEs

- References

Not all fields are mandatory, but clarity and neutrality are required.

---

## Individual vulnerabilities and population convergence

While individuals differ in genetics, experience, culture, and environment, **large-scale human behavior converges**.

CHVE is based on the observation that:

- Vulnerabilities manifest at the individual cognitive level

- Variance exists between individuals

- Predictability emerges at the population level

- Aggregate exploit success scales with exposure, independent of individual learning effects.

CHVEs document vulnerabilities that remain observable across:

- Cultures

- Age groups

- Education levels

- Socioeconomic contexts

---

## Mitigations (“human patches”)

Mitigations may include:

- Awareness and reframing

- Structural or process changes

- Slowing decision-making

- Reducing attack surface (e.g. limiting exposure)

Mitigations do **not** imply elimination — only risk reduction due to the probabilistic nature.

---

## Repository structure

```
chve/
├── README.md
├── CONTRIBUTING.md
├── GOVERNANCE.md
├── taxonomy/
│   ├── categories.md
│   └── attack-vectors.md
├── chves/
│   ├── CHVE-YYYY-NNNN.md
│   └── ...
└── tools/
    └── template.md
```

---

## Contributing

Contributions are welcome.

Please read `CONTRIBUTING.md` before submitting a CHVE. In short:

- One vulnerability per pull request

- Neutral, technical language

- Observable and exploitable patterns only

- Cite sources where possible

- Avoid ideology, politics, or personal attacks

Disagreements belong in pull request dnot pop psychologyiscussions, not in CHVE documents.

---

## License and intent

CHVE is intended for:

- Education

- Awareness

- Research

- Defensive use

It is **not** intended to enable manipulation or harm.

Documenting vulnerabilities does not create them.

---

## Closing note

CHVE treats human behavior the way security treats software:  
not as perfect,  
not as broken,  
but as **something worth understanding before it is exploited**.
