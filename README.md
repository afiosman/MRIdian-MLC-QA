### Automated Log-File-Based Quality Assurance of MLC Positional Accuracy for the ViewRay MRIdian MR-Linac

**Virginia Commonwealth University (VCU) | Department of Radiation Oncology**

**Research software | Version 1.0.0**

---

## Overview

MRIdian-MLC-QA is a Python-based research platform developed to automate the assessment of multileaf collimator (MLC) positional accuracy for the ViewRay MRIdian 0.35-T MR-guided linear accelerator.

The framework utilizes treatment plan information and machine delivery log files to evaluate planned versus log-reported MLC positions, generate quantitative QA metrics, and support longitudinal performance monitoring.

A Streamlit-based graphical user interface facilitates standardized analysis, visualization, and reporting.

## Key Features

- **Automated log-file processing:** Parsing and matching of MRIdian upper- and lower-stack delivery logs.
- **Virtual picket-fence QA:** Analysis of MLC positional accuracy across multiple gantry angles.
- **MLC positional error analysis:** Per-leaf RMS errors, maximum absolute positional errors, and overall maximum deviations.
- **Dual-stack MLC support:** Independent evaluation of the MRIdian 138-leaf MLC system.
- **Standardized QA reporting:** Automated visualization and generation of QA summaries.
- **Longitudinal monitoring:** Tracking of MLC performance across repeated QA sessions.

## Methodology

The framework was evaluated using four virtual picket-fence treatment plans generated with gantry angles of 0°, 90°, 180°, and 270°.

Each plan consisted of 11 segments with a nominal 6-mm leaf gap.

Planned MLC positions were extracted from treatment plans and compared with the corresponding log-reported leaf positions from the MRIdian delivery system.

Upper and lower MLC stacks were independently analyzed using positional error metrics.

## Preliminary Results

The initial evaluation demonstrated a maximum absolute positional deviation of ≤0.3 mm across the analyzed leaves and gantry angles.

Longitudinal analysis showed stable MLC positional performance across the two QA sessions evaluated.

These findings support the feasibility of automated log-file-based assessment of MRIdian MLC positional accuracy.

## Software Availability

The application is maintained in a private source-code repository.

Controlled access may be considered for approved research collaborations and independent validation studies, subject to institutional authorization and applicable research-use agreements.

**The underlying Python source code is not publicly distributed through this repository.**

## Intended Use and Limitations

This software is intended for research and technical evaluation.

Log-file-based verification assesses recorded machine-delivery parameters and does not independently establish the true physical positions of MLC leaves.

The software has not been established as a standalone replacement for conventional independent MLC QA measurements and should not be used for clinical decision-making without appropriate validation and institutional approval.

## Scientific Reference

Osman, A. F. I., Ma, T., Song, B., & Song, W. (2026).

*Automated Log-File-Based Quality Assurance of MLC Positional Accuracy for a Magnetic Resonance-Guided Linear Accelerator.*

Presented at the 2026 Joint AAPM–COMP Meeting, Vancouver, Canada.

## Research Collaboration

We welcome scientific collaboration focused on independent validation, multicenter evaluation, and technical development of MRIdian MLC quality assurance methodologies.

**Contact:** Alexander F. I. Osman  
Virginia Commonwealth University  
Department of Radiation Oncology

## Intellectual Property

The underlying software implementation is not distributed under an open-source license.

Access, redistribution, modification, and permitted uses of the proprietary software are subject to applicable intellectual property rights and institutional authorization.
