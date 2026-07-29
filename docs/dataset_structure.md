# Dataset structure

The complete controlled dataset is organized around BIDS-EEG 1.9.0. This public repository documents the structure but does not contain the participant directories shown below.

```text
dataset_root/
├── dataset_description.json
├── participants.tsv
├── participants.json
├── README.md
├── CHANGES
├── sub-HC001/
│   └── ses-baseline/
│       ├── eeg/
│       └── beh/
├── sub-NOCCS001/
│   ├── ses-baseline/
│   └── ses-followup/
├── sub-CCS001/
│   ├── ses-baseline/
│   └── ses-followup/
├── derivatives/
│   ├── eeglab-preproc/
│   ├── erp/
│   ├── gfp/
│   └── topomaps/
├── code/
└── docs/
```

## Naming

- Participant identifiers are newly assigned and contain no initials or dates.
- Sessions use relative labels only.
- Raw EEG, behavior, and derivatives link through anonymous participant/session identifiers.
- The source-to-public crosswalk remains private and outside all release repositories.

## Preprocessing represented in derivatives

The manuscript describes average-mastoid re-referencing, two-pass 0.1-30 Hz filtering, bad-channel detection, ASR, extended infomax ICA, ICLabel-assisted rejection, interpolation, epoching, baseline correction, and trial rejection. Derivative provenance must record the exact software version and parameter file used for each formal release.

