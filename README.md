# MRIdian-MLC-QA

### Automated Log-File-Based Quality Assurance of MLC Positional Accuracy for the ViewRay MRIdian MR-Linac

**A Python-Based Research Platform for Automated MLC QA, Standardized Reporting, and Longitudinal Performance Monitoring**

**Virginia Commonwealth University (VCU) | Department of Radiation Oncology**

**Research Software | Version 1.0.0**

---

## Overview

**MRIdian-MLC-QA** is a Python-based research platform developed to automate the assessment of multileaf collimator (MLC) positional accuracy for the ViewRay MRIdian 0.35-T magnetic resonance-guided linear accelerator (MR-Linac).

The framework analyzes treatment plan information and machine delivery log files to quantify differences between planned and log-reported MLC positions. It provides automated data processing, visualization, standardized QA reporting, and longitudinal performance monitoring.

A Streamlit-based graphical user interface enables efficient and reproducible analysis without requiring users to interact directly with the underlying Python scripts.

The platform is designed to support research into log-file-based MLC QA and the feasibility of integrating automated analysis into routine QA workflows.

## Key Features

- **Automated log-file processing:** Parsing and matching of MRIdian upper- and lower-stack delivery logs.
- **Virtual picket-fence QA:** Assessment of MLC positional accuracy across multiple gantry angles.
- **MLC positional error analysis:** Calculation of per-leaf RMS errors, per-leaf and per-segment maximum absolute positional errors, and overall maximum deviations.
- **Dual-stack MLC support:** Independent analysis of the MRIdian dual-stack, dual-focused 138-leaf MLC configuration.
- **Standardized QA reporting:** Automated generation of numerical summaries, visualizations, and QA reports.
- **Configurable QA criteria:** Evaluation of positional deviations using defined tolerance and action levels.
- **Longitudinal performance monitoring:** Tracking of MLC positional accuracy across repeated QA sessions.
- **Web-based interface:** Streamlit application supporting file upload, analysis, results visualization, and report export.

## Methodology

The framework was initially evaluated using four virtual picket-fence treatment plans generated in the ViewRay MRIdian treatment planning system.

### Test Configuration

| Parameter | Configuration |
|---|---|
| Radiotherapy system | ViewRay MRIdian 0.35-T MR-Linac |
| MLC configuration | Dual-stack, dual-focused 138-leaf MLC |
| QA technique | Virtual picket-fence test |
| Gantry angles | 0°, 90°, 180°, and 270° |
| Segments per plan | 11 |
| Nominal leaf gap | 6 mm |
| Data sources | Treatment plan information and machine delivery log files |
| Analysis | Planned versus log-reported MLC positions |

### Analysis Workflow

1. **Data acquisition:** Obtain treatment plan information and corresponding upper- and lower-stack delivery log files.
2. **Data parsing:** Extract planned and recorded delivery parameters, including MLC positions and relevant segment information.
3. **Data matching:** Associate planned and log-reported delivery segments.
4. **MLC positional analysis:** Calculate positional deviations for the upper and lower MLC stacks independently.
5. **QA evaluation:** Quantify positional error metrics and assess deviations against defined QA criteria.
6. **Reporting:** Generate QA summaries, visualizations, and standardized reports.
7. **Longitudinal monitoring:** Evaluate temporal changes in MLC positional performance across QA sessions.

## Preliminary Results

The initial investigation demonstrated the feasibility of automated log-file-based MLC positional accuracy assessment on the MRIdian system.

**Key findings:**

- The maximum absolute positional deviation across the analyzed MLC leaves was ≤0.3 mm.
- Localized deviations were observed at segments 2 and 10 and at gantry angles of 90° and 270°.
- Longitudinal evaluation across two QA sessions demonstrated stable log-reported MLC positional performance.
- The framework enabled automated identification and visualization of positional deviations relative to predefined QA thresholds.

These findings support further investigation of automated log-file-based MLC QA as a complementary component of routine and longitudinal machine quality assurance.

Importantly, agreement between planned and log-reported positions does not independently establish agreement between logged and physically delivered leaf positions.

## Publication

The methodology was presented at the **2026 Joint AAPM–COMP Annual Meeting**, held July 19–22, 2026, in Vancouver, Canada.

The conference abstract was subsequently published in the October 2026 proceedings of *Medical Physics*.

**Conference abstract:**

Osman, A. F. I., Ma, T., Song, B., & Song, W. (2026).

*Automated Log-File-Based Quality Assurance of MLC Positional Accuracy for a Magnetic Resonance-Guided Linear Accelerator.*

2026 Joint AAPM–COMP Annual Meeting, Vancouver, Canada. *Medical Physics, 53*(10), Digital Poster Viewing Abstracts.

**Published proceedings:**

[Medical Physics, Volume 53, Issue 10 (2026), e70700](https://doi.org/10.1002/mp.70700)

*The DOI identifies the published digital-poster proceedings collection.*

## Software Architecture

The research platform integrates the following components:

- **Data ingestion:** Treatment plan and MRIdian delivery log-file processing.
- **Analysis engine:** Planned-versus-log-reported MLC positional accuracy assessment.
- **QA evaluation:** Error metrics and configurable evaluation criteria.
- **Visualization:** Graphical representation of MLC positional deviations and QA results.
- **Reporting:** Automated generation and export of standardized QA reports.
- **Trend analysis:** Longitudinal monitoring of MLC positional performance.

The application is developed primarily in Python, with Streamlit providing the graphical user interface.

## Research Collaboration and Independent Validation

We welcome scientific collaborations focused on extending and independently validating automated MRIdian MLC QA methodologies.

Potential research directions include:

- Independent validation using data from additional MRIdian systems.
- Multicenter evaluation of MLC positional accuracy and reproducibility.
- Comparison of log-file-based QA findings with independent physical measurements.
- Investigation of gantry-angle-dependent and longitudinal MLC positional behavior.
- Evaluation of automated QA workflows and reporting methods.
- Collaborative scientific publications.

A multicenter validation effort is being planned to assess the reproducibility and generalizability of the methodology across institutions.

## Software Availability

The MRIdian-MLC-QA application is maintained in a private source-code repository.

The underlying Python implementation is **not publicly distributed** through this GitHub repository.

Controlled access to a hosted research version may be provided to authorized collaborators for independent evaluation and scientific validation, subject to appropriate institutional approval and research-use arrangements.

This public repository provides project information, scientific documentation, and references to the published methodology.

## Intended Use and Limitations

**For Research Use Only.**

The platform is intended for scientific research, technical evaluation, and methodological validation.

Log-file-based QA evaluates machine-reported delivery parameters and may not detect discrepancies between reported and actual physical MLC positions.

The methodology has not been independently established as a standalone replacement for conventional measurement-based MLC QA.

Clinical implementation, modification of established QA procedures, or use in clinical decision-making requires appropriate independent validation, institutional authorization, and consideration of applicable regulatory and professional requirements.

## Intellectual Property and Licensing

The source code underlying MRId
