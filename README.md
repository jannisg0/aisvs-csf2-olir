# NIST CSF 2.0 to OWASP AISVS 1.01: NIST OLIR supportive relationship mapping

[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.23777315.svg)](https://doi.org/10.5281/zenodo.23777315)

- **Informative Reference:** OWASP-AISVS-v1.01-to-CSF-v2.0 (1.0.0)
- **Status:** screened by NIST and passed validation for the National Online Informative References (OLIR) Program; to be posted in the OLIR Catalog as a candidate for public review.
- **Archived version:** https://doi.org/10.5281/zenodo.23777315

This repository contains a supportive relationship mapping (NIST IR 8477) between the NIST Cybersecurity Framework (CSF) 2.0 Core as focal document and the OWASP Artificial Intelligence Security Verification Standard (AISVS) v1.01 as reference document, prepared with the NIST OLIR template for CSF 2.0.

> **Independent work.** This is not an official OWASP mapping and is not endorsed by the OWASP Foundation or the OWASP AISVS project. "Supports" does not imply equivalent coverage: AISVS defines detailed, testable security verification requirements for AI systems, while CSF 2.0 describes cybersecurity risk management outcomes.

## Files

| File | Content |
| --- | --- |
| `data/OWASP-AISVS-v1.01-to-CSF-v2.0_1.0.0.xlsx` | Completed NIST OLIR template, identical to the file screened by NIST (authoritative version) |
| `data/OWASP-AISVS-v1.01-to-CSF-v2.0_1.0.0.csv` | Same content as CSV (UTF-8, comma-separated) |

The Zenodo record is the citable, archived version. This repository is the working copy for feedback and future versions.

## How to read a row

Each row states that an AISVS requirement (Reference Document Element) *supports* a CSF 2.0 Subcategory (Focal Document Element). The Relationship Property qualifies the relationship (NIST IR 8477, Sec. 4.2):

- **example of**: the requirement is one way to achieve the CSF outcome; the outcome can also be achieved without it.
- **integral to**: the requirement is part of achieving the CSF outcome for AI systems in scope; the outcome cannot be achieved for them without it.
- **precedes**: the requirement is a prerequisite for applying the CSF outcome, but not part of it.

In the Comments column, "ExN" refers to CSF 2.0 Implementation Example N of the Subcategory, and "Precedent" names SP 800-53 Rev. 5 controls that NIST relates to the same Subcategory (as listed in NIST IR 8596 iprd). Strength of Relationship is "N/A" because CSF 2.0 and AISVS are not lateral documents (NIST IR 8278A Rev. 1, Sec. 3.2.12).

## Coverage and scope

255 relationships between 197 of the 213 active AISVS v1.01 requirements and 32 CSF 2.0 Subcategories. AISVS requirements whose sole purpose is content safety, output reliability (e.g., hallucination) or AI trustworthiness are not mapped; mixed-purpose requirements are mapped for their security purpose only. Requirements that combine several topics are mapped as whole elements under their AISVS identifier; the Relationship Explanation states which part supports the Subcategory.

## Feedback

Please open an issue in this repository. During NIST's public review period, comments can also be sent to <olir@nist.gov>.

## License and attribution

- Mapping: (c) 2026 Jannis Groth, licensed under [CC BY-SA 4.0](LICENSE).
- AISVS requirement text (column "Reference Document Element Description"): OWASP AISVS v1.01, (c) 2025-2026 The AISVS Project, [CC BY-SA 4.0](<https://creativecommons.org/licenses/by-sa/4.0/>), source: <https://github.com/OWASP/AISVS/tree/main/1.01>. Reproduced without modification.
- CSF 2.0 Core text (column "Focal Document Element Description"): NIST CSWP 29, <https://doi.org/10.6028/NIST.CSWP.29>, a work of the U.S. Government not subject to copyright protection in the United States.

## Citation

Groth, J. (2026). OWASP-AISVS-v1.01-to-CSF-v2.0 (Version 1.0.0) [Data set]. Zenodo. <https://doi.org/10.5281/zenodo.23777315>

See also [`CITATION.cff`](CITATION.cff).
