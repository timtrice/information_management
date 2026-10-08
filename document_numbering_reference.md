# Document Numbering Reference - Scotford Refinery Project

## 1. Core Decision Logic

Two numbering systems apply during project execution:

1. **Long-form (SCT.AIM.ST.3):** Format `AA.BBCC.DDD.EEE.F`. Assigned to documents that define, describe, or govern a physical asset and will persist in ASSAI SCT_OPS after project closeout.
2. **PG-009 (MOC):** Format `[TYPE]-[DISC]--87304-##`. Assigned to project-phase deliverables uploaded to ASSAI SCT_MOD during execution.

These are not mutually exclusive. A document can carry a PG-009 number during execution and later have its content merged into a long-form master document at as-building.

## 2. The Excerpt Test (SCT.AIM.ST.3, Section 5.1)

Section 5.1 states that documents which are "brand new documents that are excerpts from existing Client critical documents" receive PG-009 numbers during the project. Examples given: electrical schedules, LDTs, SFDs, PFDs. The list is non-exhaustive ("e.g.").

These documents must be stamped: "The information contained on this document shall be transferred to master [#] during as-building."

**The test for each deliverable:**

- Does a master document already exist in SCT_OPS that this deliverable's content will merge into at closeout? If yes, PG-009 during execution.
- Is this a new, standalone document that will persist on its own in SCT_OPS? If yes, long-form number.
- Does this document serve the project only and have no post-closeout life? If yes, PG-009 (or sketch per Section 3.4.2.1).

## 3. Supporting References

### SCT.AIM.ST.3 Section 2.1 - Technical Library Criteria

A document belongs in the technical library if it serves any of these purposes: asset definition/specification, design/engineering, manufacturing/construction, quality assurance, describing functions/interfaces, safe operating, asset integrity/maintenance, installation, changes to specifications, documenting asset state, legal requirement, future modifications.

### SCT.AIM.ST.3 Section 3.4.2.1 - Sketches

Sketches are project-only documents not retained in technical repositories. The standard explicitly states the following are NOT sketches and require long-form numbers: isometrics, plans, elevations, details, schematics, loop diagrams, contour maps.

### SCT.AIM.ST.3 Section 5.1.1 - Non-Critical Documents

Two paths at closeout: (a) non-critical documents that follow issuance standards and get uploaded to SCT_OPS at IFC revision (no as-building required), or (b) sketches that are not retained.

### PG-009 - Refinery PFD/SFD Footnote

For Manufacturing (Refinery and Chemicals), project-specific PFDs on master "rolls" get PG-009 numbers. Content must be merged into the master roll at as-built. A stamp per SCT.MIDS.ST.003 is required.

### Client Clarification (Email)

SCT_OPS = steady-state repository, visible in Digital Twin. SCT_MOD = project configuration in ASSAI. Document packages (BDEP, CWP, etc.) are submitted as indexes referencing existing documents in ASSAI, not as standalone files. PG-009 governs the packaging/submission mechanism.

## 4. Deliverable Classification

### 4.1 Long-Form Number (Standalone Technical Documents to SCT_OPS)

| Deliverable | Rationale |
|---|---|
| Individual P&ID sheets | Asset definition; not sketches per 3.4.2.1 |
| Control Narrative | Asset operation/functions |
| Equipment List | Asset definition/specification |
| Pump Data Sheets (x3) | Asset specification |
| Mechanical Data Sheet - Loading Arms | Asset specification |
| Mechanical Data Sheet - Gangways | Asset specification |
| Mechanical Data Sheet - Safety Showers | Asset specification |
| 3D Model (Revit/Navisworks/AutoPlant) | Asset definition; see Section 4 storage table |
| Piping General Arrangements | Plans; not sketches per 3.4.2.1 |
| Piping Isometrics | Explicitly not sketches per 3.4.2.1 |
| Piping Line List | Asset specification (verify no existing master) |
| Piping Specialty List | Asset specification (verify no existing master) |
| Foundation Plan | Plans; not sketches per 3.4.2.1 |
| Foundation Details | Details; not sketches per 3.4.2.1 |
| Pipe Support Framing Plan | Plans; not sketches per 3.4.2.1 |
| Platform Framing Plan | Plans; not sketches per 3.4.2.1 |
| Typical Sections | Not sketches per 3.4.2.1 |
| Elevation Views | Not sketches per 3.4.2.1 |
| Framing Details | Details; not sketches per 3.4.2.1 |
| Lighting Plan and Photometrics | Plans; asset definition |
| Grounding Layout (Plans/Schematics/Details) | Schematics/plans; not sketches per 3.4.2.1 |
| Electrical Equipment Layouts/Details/Specs | Asset specification/definition |
| Area Classification | Asset definition; legal/safety requirement |
| Instrument Panel/JB Layouts | Plans; not sketches per 3.4.2.1 |
| Instrument Wiring and Loop Diagrams | Loop diagrams; not sketches per 3.4.2.1; Section 4 confirms ASSAI SCT_OPS for Refinery |
| Instrument Location Plans | Plans; not sketches per 3.4.2.1 |
| Rail Demolition Plan | Plans; asset state documentation |
| Rail General Alignment | Plans; asset definition |
| Rack Area - Paving Plan | Plans; asset definition |

### 4.2 PG-009 Number (Project Deliverables / Excerpts)

| Deliverable | PG-009 Type | Rationale |
|---|---|---|
| PFD | PFD--87304-## | Refinery master roll; explicit in PG-009 and footnote |
| P&ID Package | PIDP--87304-## | Collection wrapper per PG-009; individual sheets get long-form |
| Schedule | N/A (project management) | Not a technical document per Section 2.1 criteria |
| MDR (Master Deliverable List) | N/A (project management) | Project coordination |
| Quality Plan | N/A (project management) | Project coordination |
| Model Review Report | ERP--87304-## | Engineering Calculations/Reports per PG-009 |
| HAZOP Action Register | Risk register or similar | Project-phase safety documentation |
| Technical RFQ - Loading Arms | TBE or MR | Technical Bid Evaluation per PG-009 |
| Technical RFQ - Gangways | TBE or MR | Technical Bid Evaluation per PG-009 |
| Technical RFQ - Safety Showers | TBE or MR | Technical Bid Evaluation per PG-009 |
| Calculation Package | ERP--87304-## | Explicit in PG-009 |
| Structural MTO | Project material takeoff | Procurement-adjacent |
| Piping Bill of Material | Project material takeoff | Procurement-adjacent |
| Electrical Bill of Material | Project material takeoff | Procurement-adjacent |
| Instrument Bill of Material | Project material takeoff | Procurement-adjacent |
| I/O List | IOL--87304-## | Explicit in PG-009 |
| Instrument Index | IND--87304-## | Explicit in PG-009 |
| Electrical Cable Schedule & Routing | ESCH--87304-## | Likely excerpt of master electrical schedule; verify with client |
| Instrument Cable Schedule & Routing | Similar to ESCH | Same logic as electrical |
| Electrical Load List | Project-specific schedule | Project coordination |
| Piping Tie-in List | Project coordination | Tie-in coordination |
| Electrical Wiring Tie-in List | Project coordination | Tie-in coordination |
| Instrument Wiring Tie-in List | Project coordination | Tie-in coordination |

### 4.3 Requires Client Confirmation

| Deliverable | Question |
|---|---|
| Piping Line List | Does a master line list exist that this merges into, or is this standalone? |
| Piping Specialty List | Same question. |
| Electrical Cable Schedule & Routing | Is this an excerpt of an existing master electrical schedule? |
| Instrument Cable Schedule & Routing | Same question. |
| 3D Model | Confirm expected storage location; Section 4 shows "No reliable updated model" for Refinery. |
| Control Narrative | Confirm this is standalone and not an excerpt of an existing master. |

## 5. Open Actions

1. **Request SCT.MIDS.ST.003** from the client. Required for stamping PFDs (and potentially other excerpts) for merge-back to master rolls.
2. **Request SCT.AIM.IDX.1** (Document and Equipment Coding Index) if not already in hand. Needed to assign correct class/subclass and document type codes for long-form numbers.
3. **Request SUG.CON.MOC.F.002** (eMOC Closeout Checklist). Lists all technical document deliverables by discipline, their criticality, and storage location. Strongest reference for settling disputes.
4. **Confirm MOC applicability.** SCT.AIM.ST.3 does not define what constitutes a MOC project. If your project is not formally classified as a MOC, the PG-009 routing argument may not apply at all.
5. **Resolve grey-area items** in Section 4.3 with the client directly.
6. **Clarify with teammate** that PG-009 governs the packaging/submission mechanism through SCT_MOD, not necessarily the permanent document identity. Individual technical documents can carry long-form numbers while being submitted in PG-009 packages.
