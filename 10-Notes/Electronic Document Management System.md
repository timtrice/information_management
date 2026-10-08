---
title: Electronic Document Management System
created: 2026-04-30T11:13:13Z
modified: 2026-04-30T11:13:29Z
---

| Class     | Required | Best Practice | Not Applicable |
| --------- | -------- | ------------- | -------------- |
| Class I   |          | x             |                |
| Class II  | x        |               |                |
| Class III | x        |               |                |

An Electronic Document Management System (EDMS) is a location where data and documentation related to specific projects is stored for access by project members. Unless otherwise specified, the chosen EDMS for Market projects shall be a single SharePoint 365 Site (SharePoint). The EDMS shall be set up to utilize the built-in functionality of SharePoint without the use of 3rd party resources. However, 3rd party resources may be used to build reports and dashboards and conduct audits on a scheduled basis.

All deliverables shall be stored in the Deliverables library within SharePoint. Additional folders may exist within the Deliverables library based on confidentiality requirements.

The EDMS shall be considered the sole source of truth for Project data and documentation. Any data or controlled documents not within the EDMS shall be considered obsolete and out of date.

All documentation within the EDMS shall contain a Document Number. With the exception of transmittals, all documentation shall also have a Document Revision, Document Revision Date, and Issue Status Code. Additional metadata may also be populated to aid in identifying and differentiating deliverables, as well as provide scheduling details.

## SharePoint

Unless otherwise specified, SharePoint is the chosen EDMS for Project-controlled documentation. SharePoint allows the creation of document libraries along with storing relevant metadata for each document. All deliverables shall be stored in the EDMS. All documents shall also have required metadata fields as listed in [[Document Control Procedure#Appendix 6 Required SharePoint Metadata and Definitions|Appendix 6]] populated.

Any deliverable not in EDMS shall be considered unreliable and out-of-date.

Every deliverable shall have a filename identical to it's document number. Only alphanumeric, dash, and space characters are permitted.

Every document shall be in native format. Once a document is finalized for an internal review cycle, an identical PDF must be produced and stored in EDMS. All metadata, regardless of file format, must be identical per document.

### Libraries

#### Controlled

> [!note]
> Identify how controlled documents would be maintained within SharePoint, if so

#### Deliverables

Deliverables is a EDMS folder (henceforth referred to as "Library") considered the primary repository for all deliverables within EDMS. Library shall contain all controlled project deliverables and associated documentation (i.e., transmittals, reviewed deliverables, etc.).

See [[Document Control Procedure#Document Metadata|Document Metadata]] for required metadata that shall be tracked and maintained.

### Versioning

Library must have versioning enabled, including minor versioning.

Major versioning uses natural numbers (i.e., 1, 2, …,  ∞). Major versioning shall be used to identify when a new revision has been released for transmittal to Client, or when a deliverable review period has ended and comments closed.

Minor versions are those which SharePoint tracks to monitor changes to a deliverable between major revisions. Minor versions are rational numbers (i.e., 0.1, 0.2, 1.1, 1.2, 1.3, …,  ∞).

Versioning shall not be confused with a revision; both fields are independent. Version numbers are a SharePoint tag simply used to track the entire history of a document regardless of review cycles.

#### Minor Versions

Minor versions are kept to record changes to a document or its metadata in between revision cycles. Such metadata could be forecast issue dates, document title modifications, or other metadata that does not directly impact the status of a document. A document with a minor version (e.g., 0.4, 1.3, 3.9, etc.) is a document that has been revised since it's last official release and shall be considered "NOI" - Not Officially Issued.

When a document has been transmitted the version history shall be flattened to preserve storage space unless project specifications require maintaining this history.

### Access

Access shall be granted based on the Class of a project and Security Classification of the document. The staff of Clients, Contractors, and Subcontractors may be granted access as requested by Project management.

Project Document Control shall create an Access Log, treated as a controlled document. This log shall be maintained by Document Control to identify user access including names, email addresses, level of confidentiality and other contact information.

By default, users should be added as a Visitor for read-access only.

The Information Management team shall be given Admin rights to SharePoint, or as Hanson IT policy permits. Outside of Information Management, no member shall have privileges beyond read-access in order to protect the integrity of SharePoint.

### Checking Out and Checking In a Document

Members with read-only access are unable to check out documentation.

#### Publishing Deliverables

When a deliverable is transmitted the document must be published to create a major version. A published document must contain the transmittal to which the document and it's respective revision belong.

## Network Server (i-drive)

> [!review]

Deliverables stored within SharePoint shall be backed up on Project's shared drive, commonly referred to as the i-drive. This folder, "17-Deliverables", is located directly under the Admin directory within the project folder.

Directory "17-Deliverables" shall have subdirectories for each transmittal incoming and outgoing between Company, Client, and any Contractors or Subcontractors, even if they are not Deliverables required by Market. This folder shall contain the native and PDF version of the officially transmitted document. Where a transmittal is required by the project, the transmittal shall also be made available.

The email from the POR authorizing transmittal of the documents shall exist in PDF format.

The email notifying Company on successful transmittal of the documents shall exist in PDF format.

Depending on Client's transmittal requirements, an email may exist notifying Client of a new transmittal. This email shall also be saved in the transmittal directory in PDF format.

### Folder Organization

**Required folder structure:**

```
[SUBJECT folder]/[Discipline Code]/[Document Number]/[Revision or Status]/
```

**Example:**

```
01-Project Management/PMG/PRJ-PMG-RPT-241215/RevA/
13-Calculations/MEC/PRJ-MEC-CAL-241220/RevA/
11-Plans/CIV/PRJ-CIV-DWG-241218/Rev0/
```

[[Master Document Register|Master Document Register]]

[[Document Metadata|Document Metadata]]
