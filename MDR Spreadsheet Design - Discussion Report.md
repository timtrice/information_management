---
project-id: 25I0007
date: 2026-05-22
status: draft — in progress
---

## Purpose

The MDR (Master Document Register) spreadsheet facilitates document number creation for project 25I0007 by enforcing prescribed metadata values for each segment of a document number. It ensures consistency and prevents duplicate document numbers.

Primary reference: **JB-08-0001 — Drawing and Document Numbering Procedure**

---

## Global Rules

### Lookup Columns

Any column designated as a lookup column must have its own dedicated worksheet within the spreadsheet. Each lookup worksheet contains the **full source table** (all columns as provided in JB-08-0001) plus an additional column for the **primary key** (the concatenated display string). The MDR column references the primary key column.

### Display Format (Primary Key)

Lookup values are never displayed as bare codes. A description or definition is always appended to aid legibility. The delimiter is ` - ` (space-hyphen-space).

The general pattern is:

```
CODE + " - " + DESCRIPTION
```

The concatenated string is the **primary key** for every lookup table. A value is a duplicate only if the full concatenated string is identical — not merely if the code segment repeats.

### Deprecated / Invalid Values

All values are included in lookup tables regardless of status (deprecated, invalid, not applicable). No values are suppressed.

---

## Columns

### Discipline

- **Type:** Lookup
- **Source:** §4.8 of JB-08-0001
- **Worksheet:** Distinct lookup worksheet

Permitted values (as listed in §4.8):

| Discipline |
|---|
| General Engineering (common or multi-discipline) |
| Quality Assurance |
| Project Management |
| Engineering Management |
| Civil Engineering |
| Structural Engineering |
| Architectural |
| Process |
| HVAC |
| Plumbing |
| Piping Engineering |
| Mechanical Engineering |
| Electrical |
| Control Systems |
| Security, IT, Fire Alarm |
| Welding Quality |
| Project Controls |
| Procurement |
| Contract Management |
| Construction |
| HSE, Fire Protection, LEED |

---

### Document Title

- **Type:** Text entry (free text)
- **Source:** Provided by project management or discipline leads, per deliverable
- **Notes:** Values assigned by POR. No lookup constraint.

---

### Professional of Record (POR)

- **Type:** Text entry (free text)
- **Notes:** Also referred to as Responsible Engineer (RE). Responsible for final reviews and approvals prior to release. No lookup constraint.

---

### Numbering Schematic

- **Type:** Lookup
- **Source:** §4.1–§4.6 of JB-08-0001
- **Worksheet:** Distinct lookup worksheet
- **Notes:** Values already follow the CODE - DESCRIPTION convention.

Permitted values:

| Value |
|---|
| 4.1 - Drawings |
| 4.2 - P&IDs and AF&IDs |
| 4.3 - Piping Isometrics |
| 4.4 - EHT Isometrics |
| 4.6 - All other documents |

> Section 4.5 is intentionally omitted from the specification.

---

### Prefix

> [!important] Required for all document classes.

- **Type:** Text only; default value "LP1"
- **Source:** JB-08-0001 project identifier
- **Required:** Yes
- **Permitted values:** To be confirmed — additional options may exist beyond `LP1`

---

### Building Number

> [!important] Required for all document classes.

- **Type:** Lookup
- **Source:** §4.7 of JB-08-0001
- **Worksheet:** Distinct lookup worksheet
- **Default:** `Y - Exterior Processes/Systems`

**Concatenation:**

```
Building Number + " - " + Description
```

All entries from §4.7 are included. All three `Y` entries are distinct concatenated strings and all appear in the lookup.

---

### GECMS Drawing Code

- **Type:** Lookup
- **Applies to:** Class 4.1 drawings only
- **Source:** Attachment 1 of JB-08-0001 (§8 of Document Numbering Standard)
- **Worksheet:** Distinct lookup worksheet

**Concatenation:**

```
GECMS Drawing Code + " - " + GECMS Discipline + " (" + GECMS col 4 + ")"
```

Example: `SF - Structural (Building Structural Drawings)`

> **Note on "GECMS col 4":** In the source PDF (Attachment 1 of JB-08-0001), two columns share the identical header "GECMS" with no further label to distinguish them. In our working reference (Document Numbering Standard.md), these are differentiated as "GECMS (col 3)" and "GECMS (col 4)" based on their position in the SharePoint table. "GECMS col 4" refers to the second of these two columns — the more specific, drawing-type-level description (e.g., "Building Structural Drawings", "Air Handling Systems"). The first column (col 3) carries the broader category name (e.g., "Structural Framing", "Mechanical HVAC").

**Deduplication rule:** The concatenated string is the primary key. Rows that produce an identical concatenated string are duplicates — keep one, discard the rest. Rows with the same GECMS Drawing Code but different col 4 values produce different strings and are **not** duplicates; all are retained.

All values are included, including `XK` (Temporary Discipline — Invalid / Deprecated).

---

### Level L1

- **Type:** Lookup
- **Applies to:** Class 4.1 drawings only
- **Source:** §4.1.1 of JB-08-0001
- **Worksheet:** Distinct lookup worksheet
- **Concatenation:** `Identifier + " - " + Description`

| Identifier | Description |
|---|---|
| 0 | Outside or General |
| 1 | 1st Floor |
| 2 | 2nd Floor |
| 3 | 3rd Floor |
| 4 | 4th Floor |
| 5 | 5th Floor |
| 6 | 6th Floor |
| N | nth Floor |

---

### Level L2

- **Type:** Lookup
- **Applies to:** Class 4.1 drawings only
- **Source:** §4.1.2 of JB-08-0001
- **Worksheet:** Distinct lookup worksheet
- **Concatenation:** `Identifier + " - " + Description`

| Identifier | Description |
|---|---|
| 0 | General (Default) |
| 5 | Half Level |

---

### Level L3

- **Type:** Lookup
- **Applies to:** Class 4.1 drawings only
- **Source:** §4.1.3 of JB-08-0001
- **Worksheet:** Distinct lookup worksheet
- **Concatenation:** `Identifier + " - " + Description`

| Identifier | Description |
|---|---|
| 0 | General (Default) |
| B | Basement |
| M | Mezzanine |
| N | Interstitial |
| P | Penthouse |
| R | Roof |
| U | U/G |

---

### Sector N1

- **Type:** Lookup
- **Applies to:** Class 4.1 drawings only
- **Source:** §4.1.4 of JB-08-0001
- **Worksheet:** Distinct lookup worksheet
- **Default:** `0`
- **Notes:** No definitions or descriptions available; identifiers serve as their own primary key. Applies to plan drawings only; does not apply to Civil drawings.

Permitted values:

| Identifier |
|---|
| 0 |
| 1 |
| 2 |
| 3 |
| 4 |
| n |

---

### Sub-Sector N2

- **Type:** Lookup
- **Applies to:** Class 4.1 drawings only
- **Source:** §4.1.5 of JB-08-0001
- **Worksheet:** Distinct lookup worksheet
- **Concatenation:** `Identifier + " - " + Description`

Permitted values from §4.1.5.1:

| Identifier | Description |
|---|---|
| 0 | No sub-sector |
| A | Upper Left |
| B | Upper Right |
| C | Lower Left |
| D | Lower Right |
| P | Partial plan within a sector |

> §4.1.5.2 (Adjacent Sector): When a drawing spans multiple sectors, N1 = first sector (lower number) and N2 = last sector (higher number). This is a usage rule, not an additional lookup list.

---

### Sheet SSS — Column M

- **Type:** Lookup
- **Applies to:** Class 4.1 drawings only
- **Source:** §4.1.6 of JB-08-0001
- **Worksheet:** Distinct lookup worksheet
- **Concatenation:** `Sheet Number Range + " (" + Drawing Type + ")"`
- **Notes:** Splits are excluded; top-level ranges only.

| Sheet Number Range | Drawing Type |
|---|---|
| 000–499 | Plans / General |
| 500–599 | Elevations |
| 600–799 | Other (Risers, Block Diagrams) |
| 800–899 | Schedules |
| 900–999 | Details, Sections |

Primary key examples: `000–499 (Plans / General)`, `500–599 (Elevations)`

---

### Drawing Discipline Code — Column N

- **Type:** Fixed value with default
- **Applies to:** Class 4.2 drawings only
- **Source:** §4.2 of JB-08-0001
- **Default:** `DI - P&ID`
- **Notes:** AF&IDs (`MI`) are not used on this project.

---

### Sheet Number — Column O

- **Applies to:** Class 4.2 drawings only
- **Notes:** Not used. Remains empty.

---

### Placeholder — Column P

- **Applies to:** Class 4.2 drawings only
- **Notes:** Purpose unknown. Reserved.

---

### Sequence Number — Column Q

- **Type:** Lookup
- **Applies to:** Class 4.2 drawings only
- **Source:** §4.2.1, §4.2.2, §4.2.4, §4.2.5 of JB-08-0001
- **Worksheet:** Distinct lookup worksheet
- **Concatenation:** `Series + " (" + Area + ")"`
- **Notes:** §4.2.3 (Oligo) removed from specification. §4.2.6 and §4.2.7 not included.

#### §4.2.1 — Small Molecule

| Series | Area |
|---|---|
| 000–099 | Not Used |
| 100–199 | Rig #1 |
| 200–299 | Rig #2 |
| 300–399 | Rig #3 |
| 400–499 | Shared Process Systems |
| 500–599 | Not Used |
| 600–699 | PWEC |
| 700–799 | GMP Distributed Material |
| 800–899 | Non-GMP Distributed Utility |
| 900–999 | Waste Treatment |
| 1000–1099 | HVAC |

#### §4.2.2 — Peptide

| Series | Area |
|---|---|
| 000–099 | Distribution Headers/Common Buffers |
| 100–149 | Synthesis 1 – Step 1 |
| 150–199 | Synthesis 1 – Step 2 |
| 200–249 | Synthesis 1 – Step 3 |
| 250–299 | Synthesis 1 – Step 4 |
| 300–349 | *(Unassigned)* |
| 350–399 | *(Unassigned)* |
| 400–449 | *(Unassigned)* |
| 450–499 | *(Unassigned)* |
| 500–599 | *(Unassigned)* |
| 600–699 | Purification – Dissolve/Reverse Phase |
| 700–799 | Purification – Precipitation/Drying |
| 800–899 | Plant Utilities |
| 900–999 | Waste Treatment |
| 1000–1099 | HVAC |

#### §4.2.4 — Tank Farm / Solvent Recovery

| Series | Area |
|---|---|
| 000–099 | Distribution Headers |
| 100–199 | *(Unassigned)* |
| 200–299 | *(Unassigned)* |
| 300–399 | *(Unassigned)* |
| 400–499 | *(Unassigned)* |
| 500–599 | *(Unassigned)* |
| 600–699 | *(Unassigned)* |
| 700–799 | *(Unassigned)* |
| 800–899 | Plant Utilities |
| 900–999 | Waste Treatment |
| 1000–1099 | HVAC |

#### §4.2.5 — CUB

| Series | Area |
|---|---|
| 000–099 | Distribution |
| 100–199 | Water Pretreatment and BFW |
| 200–299 | Steam |
| 300–399 | Nitrogen |
| 400–499 | Compressed Air |
| 500–599 | Process / HVAC Cooling Water |
| 600–699 | *(Unassigned)* |
| 700–799 | HVAC Chilled Water |
| 800–899 | Misc. |
| 900–999 | HHW, Tepid Water, and Potable Water |
| 1000–1099 | HVAC |

---

## Open Items

- Discussion is ongoing. Columns beyond Sub-Sector N2 (col L) have not yet been defined.
- Column letter assignments for cols A–G (Discipline through GECMS Drawing Code) not yet confirmed.
- Prefix permitted values beyond `LP1` not yet confirmed.
