# AHTPDB: Antihypertensive Peptides Database

Welcome to the official repository for AHTPDB, a comprehensive and manually curated database of experimentally validated antihypertensive peptides (AHTPs). This resource is designed to support researchers in peptide therapeutics, hypertension biology, and computational drug discovery.

Web Server: http://crdd.osdd.net/raghava/ahtpdb/

ZENODO : https://doi.org/10.5281/zenodo.20065627

## Citation

Kumar, R., Chaudhary, K., Sharma, M., Nagpal, G., Chauhan, J. S., Singh, S., Gautam, A., & Raghava, G. P. S. (2015).
AHTPDB: a comprehensive platform for analysis and presentation of antihypertensive peptides.
Nucleic Acids Research, 43(Database issue), D956–D962. https://doi.org/10.1093/nar/gku1141


## About the Database

AHTPDB is a dedicated and comprehensive platform for systematic collection, storage, and presentation of antihypertensive peptides. It consolidates scattered experimental findings from independent research studies into a centralized platform, enabling systematic exploration of peptide sequences, structures, sources, and biological activities.

The database integrates information from:

* Literature (PubMed, ~350 research articles)
* Public repositories (ACEpepDB, BIOPEP, EROP-Moscow)


## Key Features

**Massive Dataset**

* 5978 total entries
* 1694 unique peptides
* 3364 entries with IC50 values

**Extensive Coverage**

* 35 major peptide sources (milk, egg, fish, pork, chicken, soybean, etc.)
* Peptides from natural food, fungi, algae, microorganisms, insects, and snake venom

**Rich Annotations**

Each entry includes:

* Sequence, length, molecular mass, isoelectric point
* Source of peptide (natural or synthetic)
* Inhibitory concentration (IC50) and log value (pIC50)
* Toxicity/bitterness value
* Purification technique and assay method
* In vivo animal model data and decrease in systolic blood pressure (SBP)
* PubMed ID and year of publication

**Structural Data**

* Predicted tertiary structures via PEPstr algorithm
* Secondary structure assignment using DSSP
* SMILES representations for molecular analysis
* Structures for peptides of length 2–30 residues


## Overview

AHTPDB provides experimentally validated data along with:

* ACE-inhibiting activity profiles
* Physicochemical and structural properties
* Source-specific peptide coverage
* Toxicity and bitterness annotations
* In vivo efficacy data (SBP reduction in rat models)
* Cross-references (PubMed, ACEpepDB, BIOPEP, EROP-Moscow)


### Structure Prediction

Structures were predicted using:

* **PEPstr** — de novo tertiary structure prediction for peptides (length 5–30 residues), with extended molecular dynamics simulation of 1 ns using AMBER 11
* **Custom approach** — phi/psi torsion angle restraints at 180° for di-, tri-, and tetrapeptides, followed by AMBER simulation
* **DSSP** — secondary structure assignment from predicted tertiary structures
* **Open Babel** — conversion of tertiary structures to SMILES notation


### Web Tools Integrated

**Search**
* Basic search — query any database field
* Advanced search — multi-field queries
* Peptide search — containing or exact match
* SMILES search — molecular structure-based search

**Explore / Browse**
* By source (35 major categories)
* By peptide length
* By IC50 range and units
* By physicochemical properties

**Analysis Tools**
* Smith-Waterman similarity search
* Sequence alignment
* Mapping (super-search and sub-search)
* Amino acid composition and frequency analysis
* Physicochemical property analysis
* Secondary and tertiary structure tools


### Limitations

* Structure of 36 peptides containing pyroglutamine (non-natural residue) could not be predicted due to unavailability of special force fields
* One peptide of length 81 residues was excluded from structure prediction
* Bitterness/toxicity values available for only 156 entries (limited by literature availability)
* SBP decrease values were approximated from graphs where exact values were not provided


## Applications

* Antihypertensive peptide design and discovery
* Machine learning model training for AHTP prediction
* Structure-function analysis
* Food additive safety and efficacy research
* In silico screening and drug discovery pipelines


## Contact & Authors

**Prof. Gajendra P. S. Raghava**
Email - raghava@iiitd.ac.in
IIIT Delhi


## License

This database is distributed under the
Creative Commons Attribution Non-Commercial License (CC BY-NC 4.0)

We acknowledge all researchers whose published work contributed to this dataset.
