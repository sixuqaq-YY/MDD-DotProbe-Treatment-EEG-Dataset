# MDD Dot-Probe Treatment EEG Dataset

Documentation and access materials for the manuscript *An emotional dot-probe EEG dataset in depression: adjunctive cordycepin versus standard treatment*.

Verified public repository: https://github.com/sixuqaq-YY/MDD-DotProbe-Treatment-EEG-Dataset

## Scope

The described dataset contains 64-channel EEG and behavioral data acquired during an emotional dot-probe task:

- healthy controls (HC, n = 25);
- major depressive disorder with standard treatment (NOCCS, n = 22);
- major depressive disorder with adjunctive cordycepin plus standard treatment (CCS, n = 21).

The task contains 360 trials in four blocks, using sad-neutral and fear-neutral stimulus pairs. EEG was acquired at 1000 Hz with a 0.05-100 Hz online band-pass and a 50 Hz notch filter.

## Important release boundary

This public repository contains documentation, machine-readable schemas, condition definitions, access terms, and release tooling. It does **not** contain participant EEG, clinical records, source filenames, acquisition dates, or the private identifier crosswalk.

The complete human EEG dataset is available through controlled access under a Data Use Agreement. During peer review, editors and reviewers receive a separate anonymous link to a small, de-identified representative package. See [DATA_ACCESS.md](DATA_ACCESS.md).

## Repository contents

- `dataset_description.json`: BIDS-oriented dataset metadata.
- `participants.json`: participant metadata field definitions.
- `participants_template.tsv`: synthetic examples only.
- `docs/condition_dictionary.tsv`: task conditions and trigger codes.
- `docs/treatment_arm_dictionary.tsv`: HC, NOCCS, and CCS definitions.
- `docs/visit_dictionary.tsv`: baseline and follow-up definitions.
- `docs/metadata_dictionary.tsv`: reusable metadata schema.
- `docs/dataset_structure.md`: intended BIDS-EEG and derivative layout.
- `docs/stimulus_access.md`: IAPS/CFAPS reuse restrictions.
- `docs/reviewer_access.md`: reviewer-package scope.
- `DATA_ACCESS.md`: complete-dataset access process.
- `DATA_USE_AGREEMENT.md`: proposed participant-protection terms.

## Data organization

The controlled release follows BIDS-EEG 1.9.0 for raw data and separates derived outputs by processing stage and analysis target. Public IDs do not encode initials, dates, clinical values, or treatment sequence.

## Code

Repository release and validation tools may be distributed under the MIT License. Analysis code will be advertised as available only after the authors supply and approve the exact scripts for public release.

## Citation

Use the metadata in `CITATION.cff`. A permanent dataset DOI will be added to the version of record after deposition in an approved long-term repository.

## Contact

Controlled-access enquiries: `202531061032@mail.bnu.edu.cn`
