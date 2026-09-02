Reviewed by the Oversight Committee [date]

# Metadata and technical standards

This page summarises the main metadata and technical standards used by PublicnEUro. It is an overview; the detailed machine-readable records, schemas and generated exports are maintained in the [PublicnEUro metadata repository](https://github.com/Public-nEUro/PublicnEUro-metadata).

## BIDS

PublicnEUro uses the [Brain Imaging Data Structure](https://bids.neuroimaging.io/) (BIDS) as the primary organisation and metadata standard for neuroimaging datasets. BIDS provides a consistent file and metadata structure for MRI, PET, EEG, MEG and related research data.

Datasets are expected to be valid BIDS datasets, or close enough to an applicable BIDS Extension Proposal when the relevant modality or metadata are still under active standardisation. BIDS validation supports interoperability, reuse, curation and automated catalogue generation.

## DataLad catalogue

PublicnEUro uses [DataLad](https://www.datalad.org/) for versioned data representaton management. The public catalogue describes dataset-level metadata, access conditions, DOI information, lifecycle status and retrieval information.

The catalogue and generated metadata allow users to discover datasets without direct access to participant-level data. For controlled datasets, the public record remains visible while file access is mediated through registration, Data User Agreements and any required transfer safeguards.

## Crossref DOI

The Neurobiology Research Unit is a member of [Crossref](https://www.crossref.org/) identifed with the root address https://doi.org/10.70883/. Published dataset versions receive persistent DOI identifiers so they can be cited and resolved over time. The DOI landing page points users to the public dataset record, where metadata, access conditions, lifecycle status and retrieval information can be maintained independently of immediate file availability.

## NeuroBagel

PublicnEUro supports [NeuroBagel](https://neurobagel.org/) annotations for federated participant-level discovery. Data authors are encouraged to annotate `participants.tsv` using the NeuroBagel annotation tool and provide the resulting dictionary JSON to PublicnEUro.

NeuroBagel annotations are not mandatory for every dataset, but they improve findability across compatible neuroimaging discovery systems.

## Digital Use Conditions

Digital Use Conditions (DUC) provide a structured summary of permissions, obligations and prohibitions derived from the authoritative licence or Data User Agreement. DUC records do not replace the legal text; the source licence or DUA remains authoritative.

PublicnEUro publishes DUC information in the open dataset metadata records: [PublicnEUro-metadata datasets](https://github.com/Public-nEUro/PublicnEUro-metadata/tree/main/datasets).

## JSON Schema

PublicnEUro uses JSON Schema to define the structure of dataset-level governance metadata, including versions, lifecycle status, retrieval information, DOI information and Digital Use Conditions.

The current schema is published openly at [schema/dataset.schema.json](https://github.com/Public-nEUro/PublicnEUro-metadata/blob/main/schema/dataset.schema.json).

## OpenAIRE CERIF XML

PublicnEUro exports repository metadata in OpenAIRE CERIF XML for repository-wide exchange. The export represents dataset products and their public metadata in a machine-readable XML format.

The generated OpenAIRE export is published at [exports/openaire-cerif.xml](https://github.com/Public-nEUro/PublicnEUro-metadata/blob/main/exports/openaire-cerif.xml).

## re3data XML

PublicnEUro also generates re3data XML for repository-level description. This records information about PublicnEUro as a repository, rather than replacing dataset-level metadata records.

The generated re3data export is published at [exports/re3data.xml](https://github.com/Public-nEUro/PublicnEUro-metadata/blob/main/exports/re3data.xml).
