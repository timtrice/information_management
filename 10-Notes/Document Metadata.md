---
title: Document Metadata
created: 2026-04-30T11:04:02Z
modified: 2026-04-30T11:09:59Z
---

| Class     | Required | Best Practice | Not Applicable |
| --------- | -------- | ------------- | -------------- |
| Class I   |          | x             |                |
| Class II  | x        |               |                |
| Class III | x        |               |                |

- File Name
- Document Number
- Document Title
- Revision
- Revision Date
- Issue Status Code
- Transmittal
- Transmittal Date
- Due Date
- Project Code
- Discipline Code
- Document Type Code
- POR
- TM

## Document Numbering Specifications

> [!review]

---

> [!warning]
> This may be addressed already in [[Document Control Procedure#Appendix A Document Numbering Schematic]]

**File Naming**

Every document file shall be named identically to its document number:

- Document number: `PRJ-CIV-DWG-241215`
- File name: `PRJ-CIV-DWG-241215.pdf`

---

All controlled documents shall utilize a standardized numbering system that provides systematic identification, organization, and tracking throughout the document lifecycle. This numbering system applies exclusively to Market-created documentation and does not extend to external party documents, which retain their original numbering schemes.

### Purpose and Benefits

The standardized numbering system serves multiple critical functions:

- Unique identification of every Market document within the project environment
- Systematic organization by discipline, document type, and creation sequence
- Audit trail support for document lifecycle tracking and compliance requirements
- Integration capability with Data Warehouse tools and document management systems
- Efficient retrieval through structured search and filtering capabilities

### Universal Format Application

All Market projects shall utilize the same document numbering format regardless of project classification. This approach eliminates complexity variations between project classes while maintaining systematic organization benefits across all Market activities.

### Sequential Number Management

Document sequential numbers shall be assigned using Data Warehouse tools or systematic network drive review to ensure integrity and prevent conflicts.

Sequential numbers shall follow discipline-specific implementation:

- Numbers shall be unique within each discipline/document type combination
- Numbering shall begin at 0001 for each discipline/document type combination
- VOID document numbers shall never be reused under any circumstances
- CAN document numbers shall not be reused for operational simplicity
- Sequential gaps from retired numbers remain permanent in the numbering system to avoid potential complications through project maturity.

### Lifecycle Consistency

Document numbers shall remain constant throughout the document lifecycle regardless of revision status, Issue Status Code changes, or project classification modifications. This consistency ensures reliable document identification and audit trail maintenance.

External party documents maintain their original numbering systems and are tracked through existing Company submittal and correspondence management processes as defined in applicable QUAL procedures.

Complete format specifications, code definitions, and sequential numbering rules are provided in Appendix A.

### Format Requirements

All Class I project documents shall use the following numbering format:

**AAICCCC-DDD-EEE-FFFF**

Where:

- **AABCCCC**: Project number
	- **AA**=two-digit year
	- **I**=market identifier "I" for "Industry"
	- **CCCC**=four-digit sequential number assigned by Company
- **DDD**: Discipline code (3-character)
- **EEE**: Document type code (3-character)
- **FFFF**: Sequential number (4-digit, discipline-specific)
	- Date in YYYYMMDD format may be used for Class I projects.

### Examples

- `23I0024-CIV-DWG-241215` (Project drawing created December 15, 2024)
- `25I0117-MEC-CAL-241220` (Mechanical calculation created December 20, 2024)
- `24I0201-PMG-RPT-241218` (Project management report created December 18, 2024)
- `23I0794-PMG-MIN-0023` (Project management meeting minutes with sequence 0023)

## Document Revision

Document revisions shall follow industry-standard practices based on document status and review requirements.

### Alpha Revisions

Alpha revisions shall be used for documents in review cycles:

- Sequence: A, B, C, D, E, F, G, H, J, K, L, M, N, P, Q, R, S, T, U, V, W, X, Y, Z
- Letters I and O shall not be used to prevent confusion with numbers
- If revisions exceed Z, continue with AA, AB, AC, etc.

### Numerical Revisions

Numerical revisions shall be used for approved documents:

- Sequence: 0, 1, 2, 3, 4, 5, 6, 7, 8, 9
- Begin with 0 for first approved version
- Increment sequentially for subsequent approved versions

### Mixed Revisions

Mixed revisions shall be used when approved documents require re-review:

- Format: \[Number\]\[Letter\] (e.g., 0A, 1B, 2C)
- Combines numerical base with alphabetic increment
- Used when documents return to review cycle after approval

### Revision Assignment Rules

- No revisions shall be skipped in sequence
- Each document type follows specific revision patterns based on Issue Status Code requirements (see [[Document Control Procedure#Issue Status Codes|Issue Status Codes]])

## Document Revision Date

Document revision dates shall be printed in YYYY-MM-DD format where

- YYYY - four-digit year
- MM - two-digit month
- DD - two-digit date

## Issue Status Codes

The following Issue Status Codes shall be used to identify document review status:

|Code|Description|Revision Format|Usage|
|:-:|---|:-:|---|
|PLN|Planned|N/A|Documents scheduled for creation but not yet drafted|
|DFT|Draft|Alpha|Documents in development phase|
|IFI|Issued for Information|Alpha|Documents providing information without requiring action|
|IFE|Issued for Estimate|Alpha|Documents supporting cost estimation activities|
|IFR|Issued for Review|Alpha|Documents formally distributed for review|
|IFA|Issued for Approval|Alpha|Documents ready for final approval after review|
|IFU|Issued for Use|Numerical|Documents approved for operational use|
|APP|Approved|Numerical|Documents with formal approval status|
|IFH|Issued for HAZOP|Alpha|Documents approved for HAZOP study activities|
|IFD|Issued for Design|Alpha|Documents released for design development|
|IFC|Issued for Construction|Numerical|Documents approved for construction activities|
|ASB|As Built|Numerical|Documents reflecting actual constructed conditions|
|SUP|Superseded|Next sequential|Documents replaced by newer versions|
|CAN|Cancelled|N/A|Documents no longer required (metadata tracking only)|
|REJ|Rejected|Alpha|Documents returned for revision after review|
|VOID|Void|Numerical|Documents formally voided and withdrawn|

### Issue Status Code Rules

- CAN status is used for metadata tracking only and shall not be issued as a document revision
- VOID document numbers shall never be reused under any circumstances
- Typical document progression follows: PLN → DFT → IFR → IFA → APP
- APP usage depends on client requirements and project specifications

## Return Status Codes

Return Status Codes identify client approval status for submitted documents. These codes shall be used when tracking client review responses:

|Code|Description|Typical Action|
|:-:|---|---|
|Code 1|Approved|Document may proceed to next Issue Status Code or remain as submitted|
|Code 2|Approved with comments|Document may proceed but comments should be incorporated in future revisions|
|Code 3|Rejected|Document requires revision and resubmittal|
|Code 4|No review required|Document accepted without formal review process|
|Code 5|VOID|Document formally voided by client|

### Return Status Code Application

- Return Status Codes apply only to documents submitted for external review
- Code 1 and Code 4 typically allow progression to next Issue Status Code
- Code 2 and Code 3 typically require document revision and resubmittal
- Code 5 requires document voiding and potential replacement document creation

## Transmittal

> [!todo]

## Security Classification

Each controlled document shall be assigned to a Security Classification. This Security Classification identifies storage location, distribution requirements, and access permissions.

### Security Classification Codes

| Classification        | Definition                                                                                                                                                        |
| --------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Unrestricted**      | Document can be shared within Client and other 3rd parties                                                                                                        |
| **Restricted**        | Document can be shared within Client                                                                                                                              |
| **Confidential**      | Document can be shared within market                                                                                                                              |
| **Most Confidential** | Document is highly confidential and can only be stored in a repository specially configured for that purpose. Access confined exclusively to project team members |

![[security-classification.png]]

### Default Classification

All project documents shall default to "Restricted" classification unless otherwise specified by Project Management or Client requirements.

Security Classification shall be clearly identified on the drawing or cover page of the document.
