---
created: 2026-05-18T12:08:46Z
modified: 2026-05-18T12:10:44Z
---

## Basic Document Control — Training Summary

### Purpose

This report summarizes the foundational training provided on document control (DC) and information management (IM) within the energy industry. It is intended to bring a new team member up to speed on the core concepts, terminology, processes, and rules discussed during initial training sessions. This is not exhaustive — further detail on specific procedures, workflows, and project-specific requirements will follow in subsequent training.

---

### Document Control and Information Management

#### Document Control

Document control is the practice of managing documents through their entire lifecycle: creation, review, approval, distribution, revision, and retirement. The primary goal is to ensure that all personnel are working from the correct, current version of any given document at all times.

#### Information Management

Information management is the broader discipline that encompasses document control. It includes databases, records retention schedules, metadata standards, data capture, organization, storage, security, retrieval, and disposal. Information management ensures that information flows to the right people at the right time.

Document control is a subset of information management. A document controller/information management professional is responsible for both, but document control represents the core day-to-day operational function.

---

### EDMS (Electronic Data/Document Management System)

An EDMS is the primary repository where documentation and its associated metadata are held. The organization uses Microsoft SharePoint as its primary EDMS.

#### The Golden Rule

**Only one version of a document may be visible in the EDMS, and that shall always be the latest version.**

When a document is revised, the previous version is archived behind the scenes. Users only ever see the current version. In SharePoint, this is handled through its native versioning capability — a document can be layered on top of another provided they share the same file name, with previous versions dropping into version history automatically.

#### Single Source of Truth

The EDMS shall be considered the sole source of truth. Once a deliverable is downloaded from the EDMS, it is considered invalid, no longer applicable, or outdated. No document or drawing anywhere other than the EDMS shall be considered a legitimate document.

---

### Terminology

#### Deliverables, Documents, and Drawings

- **Deliverables**: The umbrella term for all contractually obligated documents and drawings that must be submitted and approved during a project.
- **Documents**: A specific category of deliverable, such as procedures or manuals.
- **Drawings**: A specific category of deliverable, such as ISOs or wiring diagrams.

All documents and drawings are deliverables. The term "deliverables" should be used when referring to them collectively.

#### Shall, Should, and May

These terms follow legal guidelines and carry specific weight:

- **Shall**: A hard rule that must be obeyed.
- **Should**: Best practice but not required.
- **May**: At the user's discretion.

---

### Document Numbering

#### Structure

Document numbers are unique alphanumeric identifiers that differentiate one deliverable from another. The file name of a deliverable in the EDMS is typically (and as best practice) the document number itself.

The standard format is:

**[Project]-[Discipline]-[Document Type]-[Sequence]**

Example: **PRJ-MEC-PLN-0001**

- **PRJ**: Project code
- **MEC**: Discipline code (e.g., Mechanical)
- **PLN**: Document type code (e.g., Plan)
- **0001**: Sequence number

#### Rules

- No two deliverables shall share the same document number.
- The sequence number is the next available integer within a given discipline-type combination.
- Most document types are shared across disciplines, but some may exist in one or more disciplines and not others.
- The document number is metadata-driven — each segment carries meaningful information about the project, discipline, and document type.
- DC/IM has its own discipline code, and transmittals have their own document type code, following the same convention.

---

### Revisioning

#### Industry-Standard Revision Scheme

The organization follows industry-standard revision practices:

##### Review Cycle (Alpha Revisions)

Any deliverable in a review cycle receives an alpha revision in sequential order:

- First revision: **A**
- Second revision: **B**
- Third revision: **C**
- And so on through the alphabet.

Note: Some clients forbid the use of the letters "O" and "I" due to their potential confusion with the numbers 0 and 1. If applicable, this shall be documented in the project specifications and procedures.

##### Approval (Numeric Revisions)

Once a deliverable is approved, it receives a numeric revision starting at **0** (integer in string format):

- First approval: **0**
- Second approval: **1**
- Third approval: **2**

##### Re-Review of Approved Deliverables (Alphanumeric Revisions)

If an approved deliverable undergoes another review cycle, its revision becomes alphanumeric — the last approved numeric revision combined with the current alpha iteration:

- First re-review after approval at Rev 0: **0A**
- Second re-review: **0B**
- Third re-review: **0C**
- Upon re-approval: **1**

There is no rule that a deliverable cannot go directly from **0** to **1** without an intermediate review cycle.

---

### Issue Status Codes (ISC)

Issue status codes identify the purpose of a revision — why the deliverable was issued at a given point. Industry-standard terms are used. Examples include:

| Code | Meaning | Frequency |
|------|---------|-----------|
| IFR | Issued for Review | Very frequent |
| IFA | Issued for Approval | Very frequent |
| IFI | Issued for Information | Occasional |
| IFC | Issued for Construction | Project-phase dependent |
| ASB | As-Built | Project-phase dependent (never seen in planning phases) |

The codes used on a project naturally shift as the project moves through its phases. Additional issue status codes exist and will be defined in further training.

---

### Metadata Requirements

The following metadata shall be tracked in the EDMS and clearly identified on the face of the deliverable:

1. **Document number**
2. **Revision**
3. **Issue status code**
4. **Revision date** (the date the deliverable was revised)

#### Date Format

Dates shall follow ISO 9000 standards: **YYYY-MM-DD**.

#### Placement on Deliverables

The placement of metadata on deliverables varies by project and the templates provided:

- **Drawings**: Typically in the lower-right corner.
- **Documents**: Typically in the footer of the cover page.
- Many projects require the revision and document number to appear in the header or footer of all pages.
- Specific placement shall be defined in the project procedures.

Additional metadata fields exist beyond these essentials and may be covered in future training.

---

### Transmittals

#### Definition

Transmittals are indexes that list deliverables by revision being transmitted to the client for review, approval, or information. They may be treated as official documentation. For this organization, transmittals are a requirement, though some clients do not require them.

#### Transmittal Numbering

Transmittals follow the same document numbering convention as all other deliverables, using the DC/IM discipline code and a transmittal-specific document type code with their own unique sequence.

#### Critical Rule

The deliverables sent in a transmittal package shall match the transmittal precisely. Any discrepancy — a wrong revision, a missing deliverable, a mismatch in issue status codes, or any other inconsistency between the transmittal index and the actual deliverables — is an automatic rejection with a request to resubmit.

#### Transmittal Corrections

Once a deliverable has been transmitted to the client, it shall not be modified until the client has returned the reviewed deliverable. There is a narrow exception:

- If a deliverable was transmitted very recently (within approximately the past hour),
- A mistake is found that can be quickly rectified,
- The client has not yet processed the transmittal (rule of thumb: deliverables are processed within 24 hours),
- **And communication with the client permits**,

Then the client may reject the transmittal, the deliverable may be corrected, and the entire transmittal is to be modified and resubmitted. This is a rare exception, not a routine option.

---

### Return Status Codes (RSC)

When deliverables are returned from the client, they come with return status codes. These codes may vary by project and shall be clearly identified in the project specifications and procedures.

#### Typical Codes

| Code | Meaning | Implication |
|------|---------|-------------|
| **Code 1** | Approved | Depending on the deliverable milestone, if the deliverable has met its required ISC, resubmittal is not required. If it has not yet met the milestone, resubmittal is required. |
| **Code 2** | Approved with Comments | The deliverable may advance to the next ISC if required, but must be revised to incorporate comments and resubmitted to achieve Code 1 approval. Downstream deliverables that depend on this one may continue as-is. |
| **Code 3** | Rejected | The deliverable may **not** advance to the next ISC. It must be revised and resubmitted. Downstream deliverables that depend on this one are blocked until the issues are resolved. |
| **Code 4** | Information Only | No changes to be made and no review required. |
| **Code 5** | VOID | The deliverable is no longer required and may be voided in the system. (Void procedures to be discussed in future training.) |

#### Key Distinction: Code 2 Vs Code 3

- **Code 2** means the deliverable is good enough to continue working from. Associated deliverables may proceed.
- **Code 3** means there are fundamental issues. All dependent work is blocked until the deliverable is corrected. For example, a procedure cannot be written confidently if the specification it relies on has major errors.

#### ISC Progression on Resubmittal

The ISC assigned on resubmittal depends on context:

- An IFR deliverable returned Code 2 or Code 3 would typically be resubmitted as IFA.
- An IFC deliverable that is revised for any reason would still go out as IFC.

---

### DC's Role and Responsibilities

#### What DC Does

1. Uploads and maintains deliverables in the EDMS.
2. Receives transmittals from the client and updates the EDMS with return status codes.
3. Sends notification emails to the distribution team based on the discipline code of the deliverables.
4. Ensures no new revision of a deliverable is submitted until the previous version has been returned from the client (where applicable, such as IFR or IFA deliverables).
5. Ensures review cycles follow those established in the project specifications and procedures.
6. Prepares outgoing transmittals with exact accuracy.

#### What DC Does Not Do

- DC does not interpret technical content. DC does not have the discipline-specific expertise to evaluate the substance of deliverables.
- DC does not track the impact of return status codes on downstream or related deliverables. That responsibility falls to the discipline lead.
- DC does not determine whether a deliverable's content is correct or complete from a technical standpoint.

**DC is the gatekeeper of the process, not the interpreter of the content.**

---

### Summary of Key Principles

1. The EDMS is the sole source of truth. Nothing outside of it is legitimate.
2. Only one version of a deliverable shall be visible in the EDMS — always the latest.
3. Every deliverable shall clearly display its document number, revision, issue status code, and revision date.
4. Transmittals shall precisely match the deliverables in the package. Any discrepancy results in rejection.
5. Once transmitted, a deliverable shall not be modified until returned by the client (with rare, communication-dependent exceptions).
6. DC manages the process; discipline leads manage the technical content.
7. Terminology matters: "shall" is mandatory, "should" is best practice, "may" is discretionary.
