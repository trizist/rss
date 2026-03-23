# Contestable Uncertainty Interfaces for Professional AI

[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.1915418.svg)](https://doi.org/10.5281/zenodo.1915418)
[![License: CC BY 4.0](https://img.shields.io/badge/License-CC%20BY%204.0-lightgrey.svg)](http://creativecommons.org/licenses/by/4.0/)
[![Journal](https://img.shields.io/badge/Journal-RSS%3A%20Data%20Science%20%26%20AI-blue)](https://academic.oup.com/rssdat)
[![Special Issue](https://img.shields.io/badge/Special%20Issue-Uncertainty%20in%20the%20Era%20of%20AI-orange)](https://academic.oup.com/rssdat/pages/call-for-papers-uncertainty-in-the-era-of-ai)

> **Abstract:** Generative and predictive AI systems are increasingly deployed in high-stakes domains (healthcare, law, hiring) where decision-support tools shape consequential human judgment. Yet, most systems communicate uncertainty solely through confidence scores, encouraging institutional actors to treat contested interpretation as mere incomplete information. This project argues that professional AI must distinguish between **quantifiable model uncertainty** (epistemic) and **interpretive uncertainty** (hermeneutic), triggering structured human deliberation rather than offering spurious numeric closure.

This repository hosts the open-source companion materials, design specifications, and reproducibility package for the paper **"Beyond Confidence Scores: Designing Contestable Uncertainty Interfaces for High-Stakes Professional AI"** by **Umair Abbas**, submitted to *RSS: Data Science and Artificial Intelligence* (Special Issue: *Uncertainty in the Era of AI*).

## 📖 Context & Motivation

The dominant accountability problem in contemporary AI is not just model error; it is **institutional deference**—the conversion of software outputs into presumptively authoritative evidence. As highlighted by the **Post Office Horizon IT Inquiry**, treating system outputs as epistemically privileged can turn technical faults into governance failures and human injustice [^1].

Simultaneously, the **EU AI Act (Article 14)** mandates that high-risk AI systems must be designed for effective human oversight, requiring users to understand limitations, resist automation bias, and possess the capacity to **override or disregard** outputs [^2].

This project operationalizes the theoretical distinction proposed by Delacroix et al. [^3] between:
*   **Epistemic Uncertainty:** Gaps in knowledge reducible by more data (e.g., missing lab results).
*   **Hermeneutic Uncertainty:** The inherently open nature of interpretation (e.g., cultural bias in a student essay, ethical dilemmas in triage).

## 🗂️ Repository Structure

```text
.
├── manuscript/                     # Source files for the main paper
│   └── Beyond_Confidence_Scores.pdf
├── supplementary_materials/        # Additional guides and frameworks
│   ├── Technical_Design_Specification.pdf
│   ├── Operational_Framework_EU_AI_Act.pdf
│   ├── Beyond_the_Score_Guide.pdf
│   └── Case_Review_Horizon_Inquiry.pdf
├── media/                          # Audio briefing and visual assets
│   └── The_Illusion_Of_AI_Confidence_Scores.m4a
├── zenodo_metadata.json            # Metadata used for the DOI registration
├── LICENSE                         # Creative Commons Attribution 4.0 International
└── README.md                       # This file
```

## 🔑 Key Contributions

### 1. The Contestable Uncertainty Framework
We propose four design principles for high-stakes AI interfaces, aligning with the **EU AI Act's** human oversight requirements:
1.  **Differentiation:** Visually separate "low confidence" (data missing) from "contested meaning" (interpretive risk).
2.  **Deliberative Handoffs:** Replace final recommendations with "structured invitations to inquiry" when hermeneutic uncertainty is detected.
3.  **Auditability:** Immutable logging of inputs, human overrides, and rationale capture to ensure traceability.
4.  **Participatory Refinement:** Mechanisms for professional communities to iteratively define how uncertainty is expressed, preventing the ossification of professional norms.

### 2. Reproducibility Package
Aligned with *RSS: Data Science and Artificial Intelligence* data policies, this repo contains the full evidentiary basis for the paper:
*   **Case Review:** An analysis of the Post Office Horizon IT Inquiry, illustrating the transition from software errors to social injustice when contestability is absent.
*   **Operational Framework:** A guide for aligning professional workflows with EU AI Act Article 14.
*   **Technical Specifications:** Detailed UI/UX patterns for implementing dual-uncertainty displays.
*   **Audio Briefing:** A narrated summary of the core arguments for accessible consumption.

### 3. Policy Alignment
This work directly supports the implementation of:
*   **EU AI Act Article 14:** Human Oversight measures.
*   **EU AI Liability Directive:** Ensuring traceability for harm caused by AI systems.
*   **RSS Journal Standards:** Promoting openness, reproducibility, and workflow visibility.

## 🛠️ Usage & Implementation

### For Researchers
Use the `supplementary_materials/` to replicate the comparative analysis of regulatory frameworks. The **Operational Framework** maps legal requirements (e.g., EU AI Act Art. 14) to specific interface features.

### For Developers
Refer to `Technical_Design_Specification.pdf` for implementation details on building "Contestable Interfaces." Key features include:
*   **Dual-Uncertainty Display:** Rendering both probability scores and interpretive flags.
*   **Frictionless Override:** UI patterns that make rejecting AI recommendations easy but documented.
*   **Rationale Capture:** Prompting users to explain *why* they overridden a high-confidence suggestion.

### For Policymakers & Boards
The **Case Review** and **Beyond the Score Guide** provide non-technical briefings on why confidence scores are insufficient for governance and how to structure audit trails for liability protection.

## 📄 Citation

If you use this framework, data, or design specification in your research, please cite the associated Zenodo record:

> Abbas, U. (2026). *Contestable Uncertainty Interfaces for Professional AI* [Data set]. Zenodo. https://doi.org/10.5281/zenodo.1915418

**BibTeX:**
```bibtex
@misc{abbas2026contestable,
  author       = {Abbas, Umair},
  title        = {Contestable Uncertainty Interfaces for Professional AI},
  year         = {2026},
  publisher    = {Zenodo},
  doi          = {10.5281/zenodo.1915418},
  url          = {https://doi.org/10.5281/zenodo.1915418},
  note         = {Supplementary materials for manuscript submitted to RSS: Data Science and Artificial Intelligence}
}
```

## ⚖️ License

This project is open science. All documents, designs, and media are released under the **Creative Commons Attribution 4.0 International (CC BY 4.0)** license to encourage broad adoption, adaptation, and integration into open-source AI tools and policy frameworks.

See [LICENSE](LICENSE) for details.

## 🤝 Contributing & Participatory Refinement

True to the paper’s thesis, this repository is designed as a living document. We invite professionals from healthcare, education, law, and data science to:
*   Submit pull requests refining the **uncertainty taxonomy**.
*   Propose new **interface patterns** for specific domain contexts.
*   Share case studies where "confidence scores" failed to capture interpretive risk.

Please open an issue or submit a PR to participate in this collective sense-making process.

## 📬 Contact

**Umair Abbas**  
Independent Researcher | Universal Artic Solutions  
📧 umair.siddiquie@gmail.com  
🔗 [LinkedIn](https://www.linkedin.com/in/umair-siddiquie) | [Zenodo](https://zenodo.org/)

---
*"AI should extend epistemic reach but not confiscate hermeneutic responsibility."*

[^1]: Post Office Horizon IT Inquiry. (2021). *Terms of reference*. Retrieved from https://www.postofficehorizoninquiry.org.uk
[^2]: European Commission. (2024). *Regulation (EU) 2024/1689 (AI Act)*. Retrieved from https://digital-strategy.ec.europa.eu
[^3]: Delacroix, S., et al. (2025). Beyond Quantification: Navigating Uncertainty in Professional AI Systems. *RSS: Data Science and Artificial Intelligence*, 1(1), udaf002.
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
