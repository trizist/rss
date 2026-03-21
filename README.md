# Beyond Confidence Scores: Designing Contestable Uncertainty Interfaces

[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.1915418.svg)](https://doi.org/10.5281/zenodo.1915418)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Journal](https://img.shields.io/badge/Journal-RSS%3A%20Data%20Science%20%26%20AI-blue)](https://academic.oup.com/rssdat)

> **Abstract:** Generative and predictive AI systems are increasingly deployed in high-stakes domains (healthcare, law, hiring) where decision-support tools shape consequential human judgment. Yet, most systems communicate uncertainty solely through confidence scores, encouraging institutional actors to treat contested interpretation as mere incomplete information. This project argues that professional AI must distinguish between **quantifiable model uncertainty** (epistemic) and **interpretive uncertainty** (hermeneutic), triggering structured human deliberation rather than offering spurious numeric closure.

This repository hosts the open-source companion materials, data schemas, and interface prototypes for the paper **"Beyond Confidence Scores: Designing Contestable Uncertainty Interfaces for High-Stakes Professional AI"** by **Umair Abbas**, submitted to *RSS: Data Science and Artificial Intelligence* (Special Issue: *Uncertainty in the Era of AI*).

## 📖 Context & Motivation

The dominant accountability problem in contemporary AI is not just model error; it is **institutional deference**—the conversion of software outputs into presumptively authoritative evidence. As highlighted by the **Post Office Horizon IT Inquiry**, treating system outputs as epistemically privileged can turn technical faults into governance failures and human injustice.

Simultaneously, the **EU AI Act (Article 14)** mandates that high-risk AI systems must be designed for effective human oversight, requiring users to understand limitations, resist automation bias, and possess the capacity to **override or disregard** outputs.

This project operationalizes the theoretical distinction between:
*   **Epistemic Uncertainty:** Gaps in knowledge reducible by more data (e.g., missing lab results).
*   **Hermeneutic Uncertainty:** The inherently open nature of interpretation (e.g., cultural bias in a student essay, ethical dilemmas in triage).

## 🗂️ Repository Structure

```text
.
├── manuscript/               # Source files for the paper (LaTeX/Word drafts)
├── data/                     # Coding schemas and document inventory
│   ├── source_inventory.csv  # List of analyzed policy/legal/journal docs
│   └── coding_schema.json    # Methodology for comparative analysis
├── prototypes/               # Interface design specifications & mockups
│   ├── contestable_ui_spec.md
│   └── wireframes/
├── audit_tools/              # Tools for logging overrides and rationales
│   └── audit_schema.sql
├── LICENSE                   # MIT License
└── README.md                 # This file
```

## 🔑 Key Contributions

### 1. The Contestable Uncertainty Framework
We propose four design principles for high-stakes AI interfaces:
1.  **Differentiation:** Visually separate "low confidence" (data missing) from "contested meaning" (interpretive risk).
2.  **Deliberative Handoffs:** Replace final recommendations with "structured invitations to inquiry" when hermeneutic uncertainty is detected.
3.  **Auditability:** Immutable logging of inputs, human overrides, and rationale capture.
4.  **Participatory Refinement:** Mechanisms for professional communities to iteratively define how uncertainty is expressed.

### 2. Reproducibility Package
Aligned with *RSS: Data Science and Artificial Intelligence* data policies, this repo contains:
*   **Source Inventory:** Complete list of documents analyzed (EU AI Act, Horizon Inquiry Terms, RSS Editorials).
*   **Coding Schema:** The qualitative framework used to derive design principles.
*   **Interface Taxonomy:** A structured classification of uncertainty communication modes.

### 3. Empirical Study Protocol (Included)
The repository includes a full protocol (`protocols/study_design.md`) for a future mixed-methods experiment to validate these principles across HR, Healthcare, and Legal domains, measuring **automation bias**, **override quality**, and **rationale depth**.

## 🛠️ Usage & Implementation

### For Researchers
Use the `data/coding_schema.json` to replicate the comparative analysis of regulatory frameworks. The schema maps legal requirements (e.g., EU AI Act Art. 14) to specific interface features.

### For Developers
Refer to `prototypes/contestable_ui_spec.md` for implementation details on building "Contestable Interfaces." Key features include:
*   **Dual-Uncertainty Display:** Rendering both probability scores and interpretive flags.
*   **Frictionless Override:** UI patterns that make rejecting AI recommendations easy but documented.
*   **Rationale Capture:** Prompting users to explain *why* they overridden a high-confidence suggestion.

### For Policymakers & Boards
The `audit_tools/` directory provides a schema for logging decision trails, ensuring compliance with the **EU AI Act’s** traceability and human oversight mandates.

## 📄 Citation

If you use this framework, code, or data in your research, please cite the associated Zenodo record:

> Abbas, U. (2026). *Beyond Confidence Scores: Designing Contestable Uncertainty Interfaces for High-Stakes Professional AI* [Data set]. Zenodo. https://doi.org/10.5281/zenodo.1915418

**BibTeX:**
```bibtex
@misc{abbas2026contestable,
  author       = {Abbas, Umair},
  title        = {Beyond Confidence Scores: Designing Contestable Uncertainty Interfaces for High-Stakes Professional AI},
  year         = {2026},
  publisher    = {Zenodo},
  doi          = {10.5281/zenodo.1915418},
  url          = {https://doi.org/10.5281/zenodo.1915418}
}
```

## ⚖️ License

This project is open science. Code and documentation are released under the **MIT License** to encourage broad adoption and integration into open-source AI tools. Manuscript text (if included in final form) is licensed under **CC BY 4.0**.

See [LICENSE](LICENSE) for details.

## 🤝 Contributing & Participatory Refinement

True to the paper’s thesis, this repository is designed as a living document. We invite professionals from healthcare, education, law, and data science to:
*   Submit pull requests refining the **uncertainty taxonomy**.
*   Propose new **interface patterns** for specific domain contexts.
*   Share case studies where "confidence scores" failed to capture interpretive risk.

Please open an issue or submit a PR to participate in this collective sense-making process.

## 📬 Contact

**Umair Abbas**  
Independent Researcher   
📧 umair.siddiquie@gmail.com  
🔗 [LinkedIn](https://www.linkedin.com/in/umair-siddiquie) | [Zenodo](https://zenodo.org/)

---
*“AI should extend epistemic reach but not confiscate hermeneutic responsibility.”*
