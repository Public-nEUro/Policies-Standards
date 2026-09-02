Reviewed by the Oversight Committee [date]

# Preservation and dataset lifecycle

## Retention

PublicnEUro maintains dataset records so that published datasets can continue to be discovered, evaluated and cited over time. Retention of dataset files is governed by the service agreement with the data controller and by the dataset status recorded in PublicnEUro metadata.

At the end of the agreed retention period, files may remain available from PublicnEUro, move to cold storage, be returned to the data controller, or become unavailable where access must cease. Dataset metadata and DOI landing pages are maintained independently of the availability of the files.

Withdrawn records retain an appropriate public record where legally possible. This supports citation, provenance and transparency even when access to the data has stopped.

## Storage

PublicnEUro distinguishes between the public metadata record, the location of the dataset files, and the practical route for retrieval. Files may be held in online storage, cold archival storage, or outside PublicnEUro by the data controller. In some cases, no retrieval route is available.

These distinctions are represented in PublicnEUro's machine-readable metadata. The lifecycle states and retrieval fields are described in the [PublicnEUro metadata repository](https://github.com/Public-nEUro/PublicnEUro-metadata), which records for each dataset version:

- `status`: the repository lifecycle state;
- `retrieval.mode`: where and how data can currently be retrieved;
- `retrieval.url`: the normal access or external-request route, when applicable;
- `retrieval.contact`: the data-controller contact for externally held data, when applicable;
- `catalogueUrl` and `doi`: the human-readable landing page and persistent identifier.

## Published lifecycle states

For users, PublicnEUro presents five published lifecycle states:

- `active`: normally available from PublicnEUro;
- `archived`: retained in cold storage and subject to retrieval delay;
- `retired`: files are no longer held by PublicnEUro, but metadata and a controller contact remain;
- `withdrawn`: data access has ceased;
- `superseded`: a newer version or replacement should normally be used.

These user-facing lifecycle states correspond to different retrieval modes and access points listed in the metadata. A dataset version's lifecycle state does not by itself replace the licence or Data User Agreement. It explains whether the files are normally available, delayed, externally held, unavailable, or replaced.

## Retrieval modes and access points

PublicnEUro metadata separates lifecycle status from the practical retrieval route:

| Lifecycle status | Retrieval mode                                 | Access point                                                                                              |
| ---------------- | ---------------------------------------------- | --------------------------------------------------------------------------------------------------------- |
| `active`       | `online`                                     | PublicnEUro provides the normal dataset access route.                                                     |
| `archived`     | `cold_archive`                               | PublicnEUro holds the data in cold storage; retrieval is delayed.                                         |
| `retired`      | `external`                                   | PublicnEUro retains metadata but directs requests to the data controller.                                 |
| `withdrawn`    | `unavailable`                                | Data access and contact actions are intentionally unavailable.                                            |
| `superseded`   | `online`or `cold_archive`or `external` | The version may remain accessible, but a replacement identifies the version that should normally be used. |

The public catalogue and DOI landing page should therefore be read together with the retrieval metadata. The landing page identifies the dataset version, while the retrieval metadata explains whether and how files can currently be obtained.

## Metadata and DOI landing pages

Dataset metadata and DOI landing pages are maintained independently of file availability. This means that a DOI landing page can remain public for a dataset version even when the files are archived, retired, withdrawn or superseded.

Where access has ceased, the public record should explain the status in an appropriate way, subject to legal and data-protection requirements. Where a version has been superseded, the metadata should identify the newer version or replacement that should normally be cited or used.
