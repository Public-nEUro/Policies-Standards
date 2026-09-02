# Data deposit and publication

## Eligible data

PublicnEUro accepts human brain-imaging research datasets prepared using the [Brain Imaging Data Structure](https://bids.neuroimaging.io/) (BIDS). Eligible datasets may include MRI, PET, EEG, MEG and related research data, provided that the files can be organised and validated according to BIDS (or close enough if still a BIDS BEP for instance).

Upon upload, datasets are tested against the BIDS Validator. Datasets that are not valid BIDS are rejected unless the service contract states that PublicnEUro will curate the data before publication.

## Data author responsibilities

Data authors are responsible for ensuring that a service contract is in place between the author(s) and the Neurobiology Research Unit before data are uploaded. The contract sets the responsibilities of each party and the pricing of additional services provided by PublicnEUro, including data curation, private hosting, online storage and cold storage.

Data authors must also provide the dataset-specific Data User Agreement (DUA) when access control is requested. The DUA sets the licensing terms between authors and users. PublicnEUro stores signed DUAs alongside user information for the authors, but the authors and their institutions remain responsible for the legal validity of the DUA and for respecting applicable national regulations and GDPR requirements.

If data are to be shared worldwide, and depending on the DUA and transfer arrangement, data authors may also need to complete the controller-to-processor Standard Contractual Clauses.

## Required metadata

PublicnEUro represents dataset files and governance information through machine-readable metadata so that datasets can be reconstructed, discovered and evaluated without direct access to participant-level files.

Data authors must provide dataset-level metadata using the PublicnEUro record spreadsheet. This records the title, description, funders, licence and other information used on the dataset landing page and in the public catalogue.

Data authors are also encouraged to annotate `participants.tsv` with NeuroBagel using the [NeuroBagel annotation tool](https://annotate.neurobagel.org/). NeuroBagel annotations are not mandatory, but they support federated searches and can increase the visibility and impact of the dataset. When available, the NeuroBagel dictionary JSON should be sent to PublicnEUro.

Data User Agreements are converted into Digital Use Conditions used in PublicnEUro metadata records. These Digital Use Conditions are inspected by the PublicnEUro team for compatibility with data authors' regulations and are published for data author review.

## DOI assignment

Once a dataset is accepted and published, PublicnEUro publishes a presentation of the data with metadata information and assigns a DOI. The DOI supports persistent citation and links to the public dataset landing page.

## Version publication

New dataset versions can be uploaded and identified as new versions. Each published version can receive its own DOI.

At the end of the retention period specified in the contract, data can be archived in cold storage or retired and returned to the data authors. The public dataset page is maintained, with the dataset status and access conditions updated. A dataset can also be withdrawn, for example for legal reasons, while maintaining an appropriate public record where possible.

## Curation

Datasets are normally prepared by data authors in BIDS before upload. If data authors do not have the time or expertise to complete BIDS preparation themselves, PublicnEUro can provide BIDS curation as an additional paid service when this is included in the contract.

Curation and metadata enhancement are intended to improve dataset organisation, validation, discoverability and reuse. They may include BIDS validation, BIDS-related corrections, catalogue metadata checks and review of Digital Use Conditions derived from the authoritative licence or DUA.
