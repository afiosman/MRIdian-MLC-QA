# MRIdian-MLC-QA

**Automated Log-File-Based Quality Assurance of MLC Positional Accuracy for the ViewRay MRIdian MR-Linac**

**Virginia Commonwealth University | Department of Radiation Oncology**

## Overview

MRIdian-MLC-QA is a Python-based research platform developed to automate multileaf collimator (MLC) positional accuracy assessment for the ViewRay MRIdian 0.35-T MR-Linac.

The platform compares planned and log-reported MLC positions, providing quantitative QA metrics, automated reporting, and longitudinal performance monitoring through a Streamlit-based graphical interface.

<img width="1772" height="782" alt="image" src="https://github.com/user-attachments/assets/3cc91746-54e1-4f32-8b50-2e99f8df42c9" />

## Key Features

- Automated parsing and analysis of MRIdian delivery log files.
- Independent assessment of upper and lower MLC stacks (138 leaves).
- Virtual picket-fence QA at multiple gantry angles.
- Per-leaf RMS and maximum absolute positional error analysis.
- Configurable QA tolerance and action criteria.
- - Automated evaluation of MLC positional accuracy against QA tolerance and action based on AAPM TG-142 and MPPG 8.b.
- Automated QA reports and longitudinal trend analysis.

## Methodology and Results

The framework was evaluated using virtual picket-fence plans at four gantry angles (0°, 90°, 180°, and 270°), each containing 11 segments with a nominal 6-mm leaf gap.

The initial evaluation demonstrated maximum absolute MLC positional deviations of ≤0.3 mm and stable log-reported MLC performance across two QA sessions.

## Publication

**Osman, A. F. I., Ma, T., Song, B., & Song, W. (2026).**

*Automated Log-File-Based Quality Assurance of MLC Positional Accuracy for a Magnetic Resonance-Guided Linear Accelerator.*

2026 Joint AAPM–COMP Meeting, Vancouver, Canada. Published in *Medical Physics, 53*(10), Digital Poster Viewing Abstracts.

[View published conference proceedings](https://doi.org/10.1002/mp.70700)

## Software Availability and Collaboration

The Python source code is maintained in a private repository and is not publicly distributed.

Controlled access to the hosted application may be available for authorized scientific collaborations, independent validation, and multicenter research, subject to institutional approval.

Researchers interested in collaboration are welcome to contact the research team.

## Intended Use

**For research use only.** Log-file-based QA assesses machine-reported delivery parameters and does not independently verify actual physical leaf positions. The software is not established as a standalone replacement for conventional measurement-based MLC QA.

---

**Contact:** Alexander F. I. Osman  
Department of Radiation Oncology, Virginia Commonwealth University
