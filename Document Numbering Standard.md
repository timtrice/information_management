---
project-id: 25I0007
---

> Based on Specification Sections 4.1–4.7 and Attachments 1–4
> Section 4.5 is intentionally omitted from the specification.

---

## 1. Overview

| Document Class | Section | Format |
|---|---|---|
| Drawings (Non-P&ID/AF&ID/Piping ISO) | 4.1 | `LP1XX-ZZ-L1L2L3N1N2SSS` |
| P&IDs and AF&IDs | 4.2 | `LP1XX-DI-0 0000 SSS` |
| Piping Isometrics | 4.3 | `LP1XX-ZZ-YYY ZZZ-SS` |
| EHT Isometrics | 4.4 | `LP1XX-ET-ZZ-YYY ZZZ-SS` |
| All Other Documents | 4.6 | `LP1XX-TTT-DDD-SSS` |

**Project-specific conventions:**

- **Building Number (XX):** Always `Y` — Exterior Processes/Systems, WBS: TFS (§4.7)
- **Sub-Sector (N2):** Almost always `P` — Partial plan within a sector (§4.1.5)
- `LP1` is the fixed project identifier and is separate from the building number.

---

## 2. Document Class 4.1 — Drawings (Non-P&ID/AF&ID/Piping ISO)

```
LP1XX-ZZ-L1L2L3N1N2SSS
```

| Segment | Content | Description |
|---|---|---|
| LP1 | Fixed | Project identifier |
| XX | `Y` (this project) | Building Number — §4.7 |
| ZZ | GECMS code | Lilly GECMS Drawing Code — Attachment 1 |
| L1 | See §4.1.1 | Level (§4.1.1) |
| L2 | See §4.1.2 | Level (§4.1.2) |
| L3 | See §4.1.3 | Level (§4.1.3) |
| N1 | See §4.1.4 | Sector (§4.1.4) |
| N2 | See §4.1.5 | Sub-Sector (§4.1.5) |
| SSS | See §4.1.6 | Sheet (§4.1.6) |

### 2.1 Level — L1 (§4.1.1)

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

### 2.2 Level — L2 (§4.1.2)

| Identifier | Description |
|---|---|
| 0 | General (Default) |
| 5 | Half Level |

### 2.3 Level — L3 (§4.1.3)

| Identifier | Description |
|---|---|
| 0 | General (Default) |
| B | Basement |
| M | Mezzanine |
| N | Interstitial |
| P | Penthouse |
| R | Roof |
| U | U/G |

### 2.4 Sector — N1 (§4.1.4)

The following applies to plan drawings and does not apply to Civil drawings.

Each building will be broken up into sectors for larger plans. Overall plans will be sector 0.

Major sectors 1, 2, 3, 4, n will represent 1/8" scale drawings.

### 2.5 Sub-Sector / Adjacent Sector — N2 (§4.1.5)

This following applies to plan drawings and does not apply to Civil drawings.

Each sector will be broken up into four (4) sub-sectors for exploded plans (e.g., ¼" scale drawings).

Overall plans will be sub-sector 0. Sub-sectors will typically be A, B, C, D. In some instances, more granular detail may be needed. For any partial plans that require larger than ¼" scale, can use the sub-sector code of P.

#### 2.5.1 Sub-Sector (§4.1.5.1)

Drawings requiring larger scale or partial plan can utilize a sub-sector.

| Identifier | Description |
|---|---|
| 0 | No sub sector |
| A | Upper Left |
| B | Upper Right |
| C | Lower Left |
| D | Lower Right |
| P | Partial plan within a sector |

#### 2.5.2 Adjacent Sector (§4.1.5.2)

Drawings which require multiple sectors can utilize adjacent sector and can use the following convention for N1 and N2.

N1 First Sector (lower number)

N2 Last Sector (higher number)

### 2.6 Sheet Number — SSS (§4.1.6)

This is the last number that we can use to make the full drawing number unique. We will group drawings of similar types using the sheet number. Typical ranges are below. If the Lilly GECMS code would be used by more than one Fluor discipline, we will sub-divide the sheet ranges. An example of a split is shown below.

| Drawing Type | Sheet Number Range |
|---|---|
| Plans / General | 000–499 |
| &nbsp;&nbsp;Split 1 | 000–249 |
| &nbsp;&nbsp;Split 2 | 250–499 |
| Elevations | 500–599 |
| &nbsp;&nbsp;Split 1 | 500–549 |
| &nbsp;&nbsp;Split 2 | 550–599 |
| Other** | 600–799 |
| &nbsp;&nbsp;Split 1 | 600–699 |
| &nbsp;&nbsp;Split 2 | 700–799 |
| Schedules | 800–899 |
| &nbsp;&nbsp;Split 1 | 800–849 |
| &nbsp;&nbsp;Split 2 | 850–899 |
| Details, Sections | 900–999 |
| &nbsp;&nbsp;Split 1 | 900–949 |
| &nbsp;&nbsp;Split 2 | 950–999 |

** Examples: Riser and Block Diagrams

---

## 3. Document Class 4.2 — P&IDs and AF&IDs

P&ID drawings should follow the Lilly standard (Attachment 1). Specifically, refer to section three and appendix six of the document Lilly Grasslands Drawing Identification and Tagging attached to this job bulletin.

```
LP1XX-DI-0 0000 SSS
```

*Note: Spaces only shown for clarity.*

| Segment | Content | Description |
|---|---|---|
| LP1 | Fixed | Project identifier |
| XX | `Y` (this project) | Building Number (Section 4.7) |
| DI or MI | DI = P&IDs, MI = AF&IDs | Drawing Discipline Code |
| 0 | Sequential; starts at 0 | Sequential Sheet Number |
| 0000 | Fixed | Leave as 00000[^1] |
| SSS | See §4.2.1–4.2.7 | Sequence Number (Sections 4.2.1 to 4.2.5)[^2] |

### 3.1 Sequence Numbers by Facility

-4.2.3 (Oligo) has been removed from the specification.

#### 3.1.1 Small Molecule (§4.2.1)

| Series | Area |
|---|---|
| 000-099 | Not Used |
| 100-199 | Rig #1 |
| 200-299 | Rig #2 |
| 300-399 | Rig #3 |
| 400-499 | Shared Process Systems |
| 500-599 | Not Used |
| 600-699 | PWEC |
| 700-799 | GMP Distributed Material |
| 800-899 | Non-GMP Distributed Utility |
| 900-999 | Waste Treatment |
| 1000-1099 | HVAC |

#### 3.1.2 Peptide (§4.2.2)

| Series | Area |
|---|---|
| 000-099 | Distribution Headers/Common Buffers |
| 100-149 | Synthesis 1 - Step 1 |
| 150-199 | Synthesis 1 - Step 2 |
| 200-249 | Synthesis 1 - Step 3 |
| 250-299 | Synthesis 1 - Step 4 |
| 300-349 | |
| 350-399 | |
| 400-449 | |
| 450-499 | |
| 500-599 | |
| 600-699 | Purification – Dissolve/Reverse Phase |
| 700-799 | Purification – Precipitation/Drying |
| 800-899 | Plant Utilities |
| 900-999 | Waste Treatment |
| 1000-1099 | HVAC |

#### 3.1.3 Tank Farm / Solvent Recovery (§4.2.4)

| Series | Area |
|---|---|
| 000-099 | Distribution Headers |
| 100-199 | |
| 200-299 | |
| 300-399 | |
| 400-499 | |
| 500-599 | |
| 600-699 | |
| 700-799 | |
| 800-899 | Plant Utilities |
| 900-999 | Waste Treatment |
| 1000-1099 | HVAC |

#### 3.1.4 CUB (§4.2.5)

| Series | Area |
|---|---|
| 000-099 | Distribution |
| 100-199 | Water Pretreatment and BFW |
| 200-299 | Steam |
| 300-399 | Nitrogen |
| 400-499 | Compressed Air |
| 500-599 | Process / HVAC Cooling Water |
| 600-699 | |
| 700-799 | HVAC Chilled Water |
| 800-899 | Misc. |
| 900-999 | HHW, Tepid Water, and Potable Water |
| 1000-1099 | HVAC |

#### 3.1.5 Admin Lab (§4.2.6)

| Series | Area |
|---|---|
| 000-099 | Distribution Headers |
| 100-199 | QC Lab |
| 200-299 | Refrigerators / Freezers |
| 300-399 | TSMS Lab |
| 400-499 | |
| 500-599 | |
| 600-699 | |
| 700-839 | Waste/Waste Collection |
| 840-899 | Plant Utility |
| 900-999 | |
| 1000-1099 | HVAC |

#### 3.1.6 Warehouse (§4.2.7)

| Series | Area |
|---|---|
| 000-099 | Distribution Headers |
| 100-199 | Weight and Dispense/Sampling |
| 200-299 | Cold Room/Refrigerators/Freezers |
| 300-399 | Pallet Washer/Inverter |
| 400-499 | |
| 500-599 | |
| 600-699 | |
| 700-799 | |
| 800-809 | Waste Collection |
| 810-999 | Plant Utility |
| 1000-1099 | HVAC |

---

## 4. Document Class 4.3 — Piping Isometrics

Piping isometrics shall follow the convention outlined below.

*Note: Spaces only shown for clarity.*

```
LP1XX-ZZ-YYY ZZZ-SS
```

| Segment | Content | Description |
|---|---|---|
| LP1 | Fixed | Project identifier |
| XX | `0 0000` (this project) | Building Number (Section 4.7) |
| ZZ | Piping Service Code | LP100-DI-00000002, P&ID Lead Sheet 2[^3] |
| YYY | Originating P&ID Number | Sequence number from Section 4.1.4[^4] |
| ZZZ | Sequential Number | Sequential Number (001, 002, 003, etc.) |
| SS | Sequential Sheet Number | Sequential Sheet Number (01, 02, 03, etc.) |

---

## 5. Document Class 4.4 — EHT Isometrics

Electrical Heat Trace isometrics shall follow the convention outlined below.

*Note: Spaces only shown for clarity.*

```
LP1XX-ET-ZZ-YYY ZZZ-SS
```

| Segment | Content | Description |
|---|---|---|
| LP1 | Fixed | Project identifier |
| XX | `Y` (this project) | Building Number (Section 4.7) |
| ET | Fixed literal | ET – EHT Isometric Identifier |
| ZZ | Piping Service Code | LP100-DI-00000002, P&ID Lead Sheet 2[^3] |
| YYY | Originating P&ID Number | Sequence number from Section 4.1.4[^4] |
| ZZZ | Sequential Number | Sequential Number (001, 002, 003, etc.) |
| SS | Sequential Sheet Number | Sequential Sheet Number (01, 02, 03, etc.) |

---

## 6. Document Class 4.6 — All Other Documents

All other documents will follow the formula below. Tables for Fluor discipline code, and building numbers are provided. The PDDM document code can be found in the document 000.200.6660 attached to this job bulletin.

```
LP1XX-TTT-DDD-SSS
```

| Segment | Content | Description |
|---|---|---|
| LP1 | Fixed | Project identifier |
| XX | `Y` (this project) | Building Number (Section 4.7) |
| TTT | See §4.8 | Discipline Code (Section 4.8) |
| DDD | See Attachments 2–4 | Doc Code (Attachments 2, 3, or 4) |
| SSS | Sequential; starts at 001 | Sequence Number *see exception*[^5] |

**Notes:**

- Discipline codes (TTT) are unique — one code per discipline. Discipline codes not listed in §4.8 are invalid regardless of appearance in Attachments 2–4.
- Document type codes (DDD) are not globally unique. The TTT-DDD combination uniquely identifies a document type. Some DDD codes are shared across disciplines; some are specific to a discipline.
- Discipline codes **251, 252, and 295** appear in Attachments 2–4 but are absent from §4.8 and are treated as invalid.

---

## 7. Reference: Building Numbers and WBS Codes (§4.7)

| Building Number | Description | WBS Node ID |
|---|---|---|
| 00 | General | GEN |
| | Site | STE |
| 10 | Peptide Synthesis/Purification Headblock Building | PHB |
| 11 | Peptide Synthesis/Purification Manufacturing Building 1 | PP1 |
| 11 | Peptide Synthesis A Manufacturing Building 1 | SA1 |
| 11 | Peptide Synthesis B Manufacturing Building 1 | SB1 |
| 12 | Peptide Synthesis/Purification Building 1 E-Building 1 | PP1 |
| 13 | Peptide Synthesis/Purification Building 1 E-Building 2 | PP1 |
| 16 | Peptide Synthesis/Purification Manufacturing Building 2 | PP2 |
| 17 | Peptide Synthesis/Purification Building 2 E-Building 1 | PP2 |
| 18 | Peptide Synthesis/Purification Building 2 E-Building 2 | PP2 |
| 30 | Small Molecule Headblock Building 1 | SMM |
| 31 | Small Molecule Manufacturing Building 1 | SMM |
| 32 | Small Molecule Manufacturing E-Building 1 | SMM |
| 35 | Small Molecule Headblock Building 2 | SM2 |
| 36 | Small Molecule Manufacturing Building 2 | SM2 |
| 37 | Small Molecule Manufacturing E-Building 2 | SM2 |
| 40 – 49 | Tank Farm E-Buildings | Various |
| 50 | Central Utilities Building (CUB) | CUB |
| 51 | Main Switchgear Building | CUB |
| 52 | CUB Cooling Tower E-Building | CUB |
| 53 | Modular Data Center (BY LILLY) | STE |
| 55 | Fire and Rescue Center | SPG |
| 56 | Fire Pump Building | CUB |
| 58 | Truck Entrance Guardhouse | STE |
| 60 | Warehouse | WHS |
| 61 | Warehouse Freezer Building | WHS |
| 65 | Waste/Recycling Center | SPG |
| 67 | Rail Spur Operators Building | STE |
| 70 | Administrative/Laboratory Building | ALB |
| 75 | Welcome Center | SPG |
| Y | Exterior processes/systems | TFS |
| Y | Site Wide Facilities – Fire Water Tank | CUB |
| Y | Sanitary Sewer – Lift Station/Metering Station | STE |

---

## 8. Reference: GECMS Drawing Codes (Attachment 1)

| GECMS Discipline   | GECMS Drawing Code | GECMS                             | GECMS                                                        | Legacy Drawing Code |
| ------------------ | ------------------ | --------------------------------- | ------------------------------------------------------------ | ------------------- |
| Architectural      | AJ                 | Architectural Lead Sheet          | Title and Lead Sheets                                        | A0                  |
| Architectural      | AS                 | Architectural Site                | Architectural Site, Plot & Landscape Plans                   | A1                  |
| Architectural      | AS                 | Architectural Site                | Exterior Elevations                                          | A2                  |
| Architectural      | AI                 | Architectural Interiors           | Architectural Floor Plans                                    | A2                  |
| Architectural      | AI                 | Architectural Interiors           | Room Finishes                                                | A3                  |
| Architectural      | AE                 | Architectural Elements            | Architectural Elements                                       | A3                  |
| Architectural      | AI                 | Architectural Interiors           | HVAC Area Classification Plans                               | A4                  |
| Architectural      | AI                 | Architectural Interiors           | Architectural Equipment Plans                                | A4                  |
| Architectural      | AI                 | Architectural Interiors           | Reflected Ceiling Plans                                      | A4                  |
| Architectural      | AK                 | Architectural Safety              | Exterior Confined Space                                      | A5                  |
| Architectural      | AK                 | Architectural Safety              | Exterior Emergency Egress                                    | A5                  |
| Architectural      | AK                 | Architectural Safety              | Exterior Fall Protection                                     | A5                  |
| Architectural      | AK                 | Architectural Safety              | Fire and Life Safety Plans                                   | A5                  |
| Architectural      | AK                 | Architectural Safety              | Interior Confined Space                                      | A5                  |
| Architectural      | AK                 | Architectural Safety              | Interior Emergency Egress                                    | A5                  |
| Architectural      | AK                 | Architectural Safety              | Interior Fall Protection                                     | A5                  |
| Architectural      | AI                 | Architectural Interiors           | Architectural Background                                     | AB                  |
| Electrical         | EJ                 | Electrical Lead Sheet             | Title and Lead Sheets                                        | E0                  |
| Electrical         | EL                 | Electrical Lighting               | Exterior Lighting                                            | E1                  |
| Electrical         | EL                 | Electrical Lighting               | Interior Lighting                                            | E1                  |
| Electrical         | EP                 | Electrical Power                  | Exterior 120 208 V Power plans                               | E2                  |
| Electrical         | EP                 | Electrical Power                  | Interior 120 208 V Power plans                               | E2                  |
| Electrical         | EP                 | Electrical Power                  | Exterior 277 480 V Power plans                               | E3                  |
| Electrical         | EP                 | Electrical Power                  | Interior 277 480 V Power plans                               | E3                  |
| Electrical         | ES                 | Electrical Site                   | Exterior Substations and Over 600V Power                     | E4                  |
| Electrical         | ES                 | Electrical Site                   | Interior Substations and Over 600V Power                     | E4                  |
| Electrical         | EK                 | Electrical Wiring Diagrams        | Exterior Wiring Diagrams                                     | E5                  |
| Electrical         | EK                 | Electrical Wiring Diagrams        | Interior Wiring Diagrams                                     | E5                  |
| Electrical         | TY                 | Telecommunications Security       | Access Control Systems                                       | E6                  |
| Telecommunications | TN                 | Telecommunications Data           | Exterior Wiring for all Communications                       | E6                  |
| Fire Protection    | FA                 | Fire Detection and Alarm          | Fire Alarm Systems                                           | E6                  |
| Telecommunications | TN                 | Telecommunications Data           | Interior Wiring for Communications                           | E6                  |
| Electrical         | EK                 | Electrical Hazardous Area         | Exterior Electrical Hazardous Area Classification            | E8                  |
| Electrical         | EK                 | Electrical Hazardous Area         | Interior Electrical Hazardous Area Classification            | E8                  |
| Mechanical         | MJ                 | Mechanical HVAC                   | Title and Lead Sheets                                        | H0                  |
| Mechanical         | MH                 | Mechanical HVAC                   | HVAC Control System Architecture                             | H1                  |
| Mechanical         | MH                 | Mechanical HVAC                   | HVAC Control Power Distribution                              | H2                  |
| Mechanical         | MH                 | Mechanical HVAC                   | HVAC Control Panel Construction                              | H3                  |
| Mechanical         | MH                 | Mechanical HVAC                   | HVAC Control Wiring Typicals                                 | H4                  |
| Mechanical         | MH                 | Mechanical HVAC                   | HVAC Control Electrical Installation Details                 | H5                  |
| Mechanical         | MH                 | Mechanical HVAC                   | HVAC Control Device Mounting Details                         | H6                  |
| Mechanical         | MH                 | Mechanical HVAC                   | HVAC Control Instrument, Electrical, and Pneumatic Locations | H7                  |
| Mechanical         | MJ                 | Mechanical Lead Sheets            | Title and Lead Sheets                                        | M0                  |
| Mechanical         | MP                 | Mechanical Piping                 | Exterior Service Piping                                      | M1                  |
| Mechanical         | MP                 | Mechanical Piping                 | Interior Service Piping                                      | M1                  |
| Process            | DP                 | Process Piping                    | Leak Detection and Repair                                    | M10                 |
| Process            | DP                 | Process Piping                    | Exterior Process Piping                                      | M2                  |
| Process            | DP                 | Process Piping                    | Interior Process Piping                                      | M2                  |
| Process            | DR                 | Process Drains and Reclaims       | Interior Sewers and Process Waste Piping Systems             | M3                  |
| Mechanical         | MH                 | Mechanical HVAC                   | Air Handling Systems                                         | M4                  |
| Mechanical         | MI                 | Mechanical Instrumentation        | HVAC Instrumentation                                         | M5                  |
| Process            | DI                 | Process Instrumentation           | Flowsheets and Piping and Instrumentation Diagram            | M6                  |
| Fire Protection    | FX                 | Fire Supression                   | Fire Protection                                              | M7                  |
| Mechanical         | MS                 | Mechanical Site                   | Cathodic Protection for Piping and Equipment                 | M8                  |
| Process            | DI                 | Process Instrumentation           | Process Engineering Flow Diagram (Internal)                  | M9                  |
| Process            | DJ                 | Process Lead Sheets               | Title and Lead Sheets                                        | P0                  |
| Process            | DE                 | Process Electrical                | Power Distribution, Wire Numbers, and Panel Numbers          | P1                  |
| Process            | DE                 | Process Electrical                | Electrical Installation Details                              | P10                 |
| Process            | DE                 | Process Electrical                | Electrical Raceway                                           | P11                 |
| Process            | DV                 | Process Vacuum                    | Pneumatic Control Loops                                      | P12                 |
| Process            | DV                 | Process Vacuum                    | Pneumatic Raceway                                            | P14                 |
| Process            | DK                 | Process                           | Instrumentation Mechanical Installation Details              | P15                 |
| Process            | DK                 | Process                           | System Architecture                                          | P2                  |
| Process            | DK                 | Process                           | Panel Construction Drawings                                  | P4                  |
| Process            | DK                 | Process                           | System Configuration                                         | P5                  |
| Process            | DK                 | Process                           | Input Output Wiring                                          | P6                  |
| Process            | DK                 | Process                           | Serial Parallel Device Interface and Cabling                 | P7                  |
| Process            | DQ                 | Process Equipment                 | Loop Typical Wiring                                          | P8                  |
| Structural         | SJ                 | Structural Lead Sheets            | Title and Lead Sheets                                        | S0                  |
| Structural         | SF                 | Structural Framing                | Building Structural Drawings                                 | S1                  |
| Structural         | SF                 | Structural Framing                | Exterior Structural Elements for Waste Treatment             | S2                  |
| Plumbing           | PS                 | Plumbing Site                     | Sewers and Process Waste Piping Systems                      | S3                  |
| Survey/Mapping     | VU                 | Survey Mapping Combined Utilities | Surveys                                                      | S4                  |
| Civil              | CP                 | Civil Paving                      | Parking Lots                                                 | S5                  |
| Civil              | CI                 | Civil Improvements                | Other Structures                                             | S6                  |
| Civil              | CS                 | Civil Site                        | Structural Elements for Non-Building Structures              | S7                  |
| Other Disciplines  | XK                 | Temporary Discipline              | Undetermined Temp Discipline                                 | U1                  |
| Other Disciplines  | XK                 | Temporary Discipline              | Invalid                                                      | A6                  |
| Other Disciplines  | XK                 | Temporary Discipline              | Invalid                                                      | A7                  |
| Mechanical         | MI                 | Mechanical Instrumentation        | Instrumentation                                              | C0                  |
| Mechanical         | MI                 | Mechanical Instrumentation        | Instrumentation                                              | C1                  |
| Mechanical         | MI                 | Mechanical Instrumentation        | Instrumentation                                              | C2                  |
| Mechanical         | XK                 | Mechanical Instrumentation        | Instrumentation                                              | C3                  |
| Mechanical         | MI                 | Mechanical Instrumentation        | Instrumentation                                              | C4                  |
| Mechanical         | MI                 | Mechanical Instrumentation        | Instrumentation                                              | C5                  |
| Mechanical         | MI                 | Mechanical Instrumentation        | Instrumentation                                              | C6                  |
| Mechanical         | MI                 | Mechanical Instrumentation        | Instrumentation                                              | C7                  |
| Other Disciplines  | XK                 | Temporary Discipline              | Invalid                                                      | E7                  |
| Other Disciplines  | XK                 | Temporary Discipline              | Invalid                                                      | E9                  |
| Other Disciplines  | XK                 | Temporary Discipline              | Deprecated                                                   | H8                  |
| Other Disciplines  | XK                 | Temporary Discipline              | Deprecated                                                   | H9                  |
| Other Disciplines  | XK                 | Temporary Discipline              | Invalid                                                      | M11                 |
| Other Disciplines  | XK                 | Temporary Discipline              | Not Applicable                                               | NA                  |
| Other Disciplines  | XK                 | Temporary Discipline              | Invalid                                                      | P13                 |
| Other Disciplines  | XK                 | Temporary Discipline              | Deprecated                                                   | P3                  |
| Other Disciplines  | XK                 | Temporary Discipline              | Deprecated                                                   | P9                  |

---

## 9. Reference: Discipline Codes (§4.8)

| Code | Discipline |
|---|---|
| 000 | General Engineering (common or multi-discipline) |
| 042 | Quality Assurance |
| 100 | Project Management |
| 200 | Engineering Management |
| 210 | Civil Engineering |
| 215 | Structural Engineering |
| 220 | Architectural |
| 225 | Process |
| 235 | HVAC |
| 240 | Plumbing |
| 250 | Piping Engineering |
| 255 | Mechanical Engineering |
| 265 | Electrical |
| 270 | Control Systems |
| 275 | Security, IT, Fire Alarm |
| 285 | Welding Quality |
| 300 | Project Controls |
| 400 | Procurement |
| 430 | Contract Management |
| 500 | Construction |
| 653 | HSE, Fire Protection, LEED |

---

## 10. Reference: Document Type Codes (Attachments 2–4)

Discipline codes 251, 252, and 295 appear in Attachments 2–4 but are absent from §4.8 and are treated as invalid. Their entries are excluded below.

### 100 – Project Management

| Document Type (DOCTYPE) | Discipline (DISCIPLINE) | Document Code (DOCCODE) | Description |
|---|---|---|---|
| 100-AQP-001 | 100 | AQP | ACTIVITY QUALITY PLAN |
| 100-ASL-001 | 100 | ASL | AUTHORIZED SIGNATURE LIST |
| 100-BID-001 | 100 | BID | BID TAB |
| 100-CFN-001 | 100 | CFN | CONFERENCE NOTE |
| 100-COR-001 | 100 | COR | CORRESPONDENCE - EXTERNAL |
| 100-DBK-001 | 100 | DBK | DATA BOOK |
| 100-DCN-001 | 100 | DCN | DESIGN CHANGE NOTICE |
| 100-DDM-001 | 100 | DDM | DOCUMENT DISTRIBUTION MATRIX |
| 100-DEV-001 | 100 | DEV | DEVIATION |
| 100-DIS-001 | 100 | DIS | DISCUSSION CONFIRMATION |
| 100-FAX-001 | 100 | FAX | FAX |
| 100-GEN-001 | 100 | GEN | GENERAL DOCUMENT |
| 100-IAG-001 | 100 | IAG | INTERFACE AGREEMENT |
| 100-IOC-001 | 100 | IOC | INTEROFFICE CORRESPONDENCE |
| 100-JOB-001 | 100 | JOB | JOB BULLETIN |
| 100-LST-001 | 100 | LST | LIST - LOG - REGISTER |
| 100-LTR-001 | 100 | LTR | LETTER |
| 100-MOM-001 | 100 | MOM | MINUTES OF MEETING |
| 100-MPR-001 | 100 | MPR | MONTHLY PROGRESS REPORT |
| 100-NDA-001 | 100 | NDA | NON-DISCLOSURE ACKNOWLEDGEMENT |
| 100-ORG-001 | 100 | ORG | ORGANIZATION CHART |
| 100-OVR-001 | 100 | OVR | OVERTIME REQUEST |
| 100-PAF-001 | 100 | PAF | PERSONNEL AUTHORIZATION FORM |
| 100-PEP-001 | 100 | PEP | PROJECT EXECUTION PLAN |
| 100-PEX-001 | 100 | PEX | PROJECT EXPERIENCES |
| 100-PPM-001 | 100 | PPM | PROJECT PROCEDURE MANUAL |
| 100-PRC-001 | 100 | PRC | PROCEDURE |
| 100-PRO-001 | 100 | PRO | PROCUREMENT DOCUMENT |
| 100-PTD-001 | 100 | PTD | PROJECT TELEPHONE DIRECTORY - LIST |
| 100-RFl-001 | 100 | RFI | REQUEST FOR INFORMATION |
| 100-RFP-001 | 100 | RFP | REQUEST FOR PROPOSAL |
| 100-RFQ-001 | 100 | RFQ | REQUEST FOR QUOTATION |
| 100-RPT-001 | 100 | RPT | REPORT - STUDY |
| 100-RSM-001 | 100 | RSM | RESUME |
| 100-SLA-001 | 100 | SLA | SERVICE LEVEL AGREEMENT |
| 100-SOW-001 | 100 | SOW | SCOPE OF WORK |
| 100-SWA-001 | 100 | SWA | STOP WORK AUTHORITY |
| 100-TEQ-001 | 100 | TEQ | TECHNICAL QUERY |
| 100-TOC-001 | 100 | TOC | TABLE OF CONTENTS |
| 100-TRA-001 | 100 | TRA | TRAVEL AUTHORIZATION |
| 100-TRN-001 | 100 | TRN | TRANSMITTAL |
| 100-TRR-001 | 100 | TRR | TRIP REQUEST |
| 100-TXP-001 | 100 | TXP | TECHNICAL EXCEPTION |
| 100-VIP-001 | 100 | VIP | VALUE IMPROVING PRACTICE |
| 100-WSR-001 | 100 | WSR | WORK STOPPAGE RECORD |

### 200 – Engineering Management

| Document Type (DOCTYPE) | Discipline (DISCIPLINE) | Document Code (DOCCODE) | Description |
|---|---|---|---|
| 200-DBK-001 | 200 | DBK | PROJECT DATA BOOK |
| 200-DCN-001 | 200 | DCN | DESIGN CHANGE NOTICE |
| 200-DTA-001 | 200 | DTA | DATABASE |
| 200-FDN-001 | 200 | FDN | FLOW DIAGRAM CHANGE NOTICE |
| 200-IOM-001 | 200 | IOM | INSTALLATION OPERATION AND MAINTENANCE MANUAL |
| 200-LST-001 | 200 | LST | LIST |
| 200-MDR-001 | 200 | MDR | PROJECT MASTER DOCUMENT REGISTER |
| 200-RPT-001 | 200 | RPT | REPORT |
| 200-TVR-001 | 200 | TVR | TURNOVER DOSSIER |

### 210 – Civil Engineering

| Document Type (DOCTYPE) | Discipline (DISCIPLINE) | Document Code (DOCCODE) | Description |
|---|---|---|---|
| 210-AUT-001 | 210 | AUT | AUTHORITY |
| 210-CAL-001 | 210 | CAL | CALCULATION |
| 210-CON-001 | 210 | CON | CONTRACT |
| 210-CWP-001 | 210 | CWP | CONSTRUCTION WORK PACKAGE |
| 210-DBD-001 | 210 | DBD | DESIGN BASIS AND CRITERIA |
| 210-DBK-001 | 210 | DBK | PROJECT DATA BOOK |
| 210-DEM-001 | 210 | DEM | DEMOLITION |
| 210-DIA-001 | 210 | DIA | DIAGRAM |
| 210-DTL-001 | 210 | DTL | DETAILS |
| 210-GAD-001 | 210 | GAD | GENERAL ARRANGEMENT DRAWING |
| 210-LST-001 | 210 | LST | LIST |
| 210-MTO-001 | 210 | MTO | MATERIAL TAKE OFF |
| 210-PLN-001 | 210 | PLN | PLAN |
| 210-PRO-001 | 210 | PRO | PROCUREMENT |
| 210-RPT-001 | 210 | RPT | REPORT |
| 210-SKT-001 | 210 | SKT | SKETCH |
| 210-SPC-001 | 210 | SPC | SPECIFICATION |
| 210-STD-001 | 210 | STD | STANDARD |

### 215 – Structural Engineering

| Document Type (DOCTYPE) | Discipline (DISCIPLINE) | Document Code (DOCCODE) | Description |
|---|---|---|---|
| 215-AUT-001 | 215 | AUT | AUTHORITY |
| 215-CAL-001 | 215 | CAL | CALCULATION |
| 215-CON-001 | 215 | CON | CONTRACT |
| 215-CWP-001 | 215 | CWP | CONSTRUCTION WORK PACKAGE |
| 215-DBD-001 | 215 | DBD | DESIGN BASIS AND CRITERIA |
| 215-DBK-001 | 215 | DBK | PROJECT DATA BOOK |
| 215-DEM-001 | 215 | DEM | DEMOLITION |
| 215-DTL-001 | 215 | DTL | DETAILS |
| 215-GAD-001 | 215 | GAD | GENERAL ARRANGEMENT DRAWING |
| 215-LST-001 | 215 | LST | LIST |
| 215-MTO-001 | 215 | MTO | MATERIAL TAKE OFF |
| 215-PLN-001 | 215 | PLN | PLAN |
| 215-PRO-001 | 215 | PRO | PROCUREMENT |
| 215-RPT-001 | 215 | RPT | REPORT |
| 215-SCH-001 | 215 | SCH | SCHEDULE |
| 215-SKT-001 | 215 | SKT | SKETCH |
| 215-SPC-001 | 215 | SPC | SPECIFICATION |
| 215-STD-001 | 215 | STD | STANDARD |

### 220 – Architectural

| Document Type (DOCTYPE) | Discipline (DISCIPLINE) | Document Code (DOCCODE) | Description |
|---|---|---|---|
| 220-AUT-001 | 220 | AUT | AUTHORITY |
| 220-CAL-001 | 220 | CAL | CALCULATION |
| 220-CON-001 | 220 | CON | CONTRACT |
| 220-CWP-001 | 220 | CWP | CONSTRUCTION WORK PACKAGE |
| 220-DBD-001 | 220 | DBD | DESIGN BASIS AND CRITERIA |
| 220-DBK-001 | 220 | DBK | PROJECT DATA BOOK |
| 220-DEM-001 | 220 | DEM | DEMOLITION |
| 220-DIA-001 | 220 | DIA | DIAGRAM |
| 220-DTL-001 | 220 | DTL | DETAILS |
| 220-ELE-001 | 220 | ELE | ELEVATION |
| 220-LST-001 | 220 | LST | LIST |
| 220-MTO-001 | 220 | MTO | MATERIAL TAKE OFF |
| 220-PLN-001 | 220 | PLN | PLAN |
| 220-PRO-001 | 220 | PRO | PROCUREMENT |
| 220-RPT-001 | 220 | RPT | REPORT |
| 220-SCH-001 | 220 | SCH | SCHEDULE |
| 220-SEC-001 | 220 | SEC | SECTION |
| 220-SMP-001 | 220 | SMP | SAMPLE |
| 220-SPC-001 | 220 | SPC | SPECIFICATION |
| 220-STD-001 | 220 | STD | STANDARD |
| 220-VIS-001 | 220 | VIS | VISUALISATION |

### 225 – Process

| Document Type (DOCTYPE) | Discipline (DISCIPLINE) | Document Code (DOCCODE) | Description |
|---|---|---|---|
| 225-CAL-001 | 225 | CAL | CALCULATION |
| 225-DBD-001 | 225 | DBD | DESIGN BASIS AND CRITERIA |
| 225-DBK-001 | 225 | DBK | PROJECT DATA BOOK |
| 225-DIA-001 | 225 | DIA | DIAGRAM |
| 225-LST-001 | 225 | LST | LIST |
| 225-NAR-002 | 225 | NAR | NARRATIVE |
| 225-PFD-001 | 225 | PFD | PROCESS FLOW DIAGRAM |
| 225-PHL-001 | 225 | PHL | PHILOSOPHY |
| 225-PID-001 | 225 | PID | PIPING AND INSTRUMENTATION DIAGRAM |
| 225-RPT-001 | 225 | RPT | REPORT |
| 225-SUM-001 | 225 | SUM | SUMMARY |

### 250 – Piping Engineering

| Document Type (DOCTYPE) | Discipline (DISCIPLINE) | Document Code (DOCCODE) | Description |
|---|---|---|---|
| 250-PLN-001 | 250 | PLN | PLAN |
| 250-PPL-001 | 250 | PPL | PLOT PLANS |
| 250-PRO-001 | 250 | PRO | PROCUREMENT |
| 250-SKT-001 | 250 | SKT | SKETCH |
| 250-SPC-001 | 250 | SPC | SPECIFICATION |
| 250-STD-001 | 250 | STD | STANDARD |
| 250-TIE-001 | 250 | TIE | TIE-IN |

### 255 – Mechanical Engineering

| Document Type (DOCTYPE) | Discipline (DISCIPLINE) | Document Code (DOCCODE) | Description |
|---|---|---|---|
| 255-AUT-001 | 255 | AUT | AUTHORITY |
| 255-CAL-001 | 255 | CAL | CALCULATION |
| 255-CON-001 | 255 | CON | CONTRACT |
| 255-CWP-001 | 255 | CWP | CONSTRUCTION WORK PACKAGE |
| 255-DBD-001 | 255 | DBD | DESIGN BASIS AND CRITERIA |
| 255-DBK-001 | 255 | DBK | PROJECT DATA BOOK |
| 255-DEM-001 | 255 | DEM | DEMOLITION |
| 255-DST-001 | 255 | DST | DATASHEET |
| 255-DTL-001 | 255 | DTL | DETAILS |
| 255-LAY-001 | 255 | LAY | LAYOUT |
| 255-LST-001 | 255 | LST | LIST |
| 255-MSD-001 | 255 | MSD | MATERIAL SELECTION DIAGRAM |
| 255-MTO-001 | 255 | MTO | MATERIAL TAKE OFF |
| 255-PFD-001 | 255 | PFD | PROCESS FLOW DIAGRAM |
| 255-PRO-001 | 255 | PRO | PROCUREMENT |
| 255-RPT-001 | 255 | RPT | REPORT |
| 255-SKT-001 | 255 | SKT | SKETCH |
| 255-SPC-001 | 255 | SPC | SPECIFICATION |
| 255-STD-001 | 255 | STD | STANDARD |

### 265 – Electrical

| Document Type (DOCTYPE) | Discipline (DISCIPLINE) | Document Code (DOCCODE) | Description |
|---|---|---|---|
| 265-AUT-001 | 265 | AUT | AUTHORITY |
| 265-CAL-001 | 265 | CAL | CALCULATION |
| 265-CON-001 | 265 | CON | CONTRACT |
| 265-CPR-001 | 265 | CPR | CONSTRUCTION POWER |
| 265-CWP-001 | 265 | CWP | CONSTRUCTION WORK PACKAGE |
| 265-DBD-001 | 265 | DBD | DESIGN BASIS AND CRITERIA |
| 265-DBK-001 | 265 | DBK | PROJECT DATA BOOK |
| 265-DEM-001 | 265 | DEM | DEMOLITION |
| 265-DIA-001 | 265 | DIA | DIAGRAM |
| 265-DST-001 | 265 | DST | DATASHEET |
| 265-DTL-001 | 265 | DTL | DETAILS |
| 265-HAC-001 | 265 | HAC | HAZARDOUS AREA CLASSIFICATION |
| 265-HTX-001 | 265 | HTX | ELECTRICAL HEAT TRACING |
| 265-LAY-001 | 265 | LAY | LAYOUT |
| 265-LST-001 | 265 | LST | LISTS |
| 265-MTO-001 | 265 | MTO | MATERIAL TAKE OFF |
| 265-PRC-001 | 265 | PRC | PROCEDURE |
| 265-PRO-001 | 265 | PRO | PROCUREMENT |
| 265-RPT-001 | 265 | RPT | REPORT |
| 265-SKT-001 | 265 | SKT | SKETCH |
| 265-SLD-001 | 265 | SLD | SINGLE LINE DIAGRAM |
| 265-SPC-001 | 265 | SPC | SPECIFICATION |
| 265-STD-001 | 265 | STD | STANDARD |

### 270 – Control Systems

| Document Type (DOCTYPE) | Discipline (DISCIPLINE) | Document Code (DOCCODE) | Description |
|---|---|---|---|
| 270-AUT-001 | 270 | AUT | AUTHORITY |
| 270-CAE-001 | 270 | CAE | CAUSE AND EFFECT DRAWING |
| 270-CAL-001 | 270 | CAL | CALCULATION |
| 270-CON-001 | 270 | CON | CONTRACT |
| 270-CWP-001 | 270 | CWP | CONSTRUCTION WORK PACKAGE |
| 270-DBD-001 | 270 | DBD | DESIGN BASIS AND CRITERIA |
| 270-DBK-001 | 270 | DBK | PROJECT DATA BOOK |
| 270-DEM-001 | 270 | DEM | DEMOLITION |
| 270-DIA-001 | 270 | DIA | DIAGRAM |
| 270-DST-001 | 270 | DST | DATASHEET |
| 270-DTL-001 | 270 | DTL | DETAILS |
| 270-LAY-001 | 270 | LAY | LAYOUT |
| 270-LST-001 | 270 | LST | LIST |
| 270-MTO-001 | 270 | MTO | MATERIAL TAKE OFF |
| 270-PRC-001 | 270 | PRC | PROCEDURE |
| 270-PRO-001 | 270 | PRO | PROCUREMENT |
| 270-RPT-001 | 270 | RPT | REPORT |
| 270-SKT-001 | 270 | SKT | SKETCH |
| 270-SPC-001 | 270 | SPC | SPECIFICATION |
| 270-STD-001 | 270 | STD | STANDARD |

### 275 – Security, IT, Fire Alarm

| Document Type (DOCTYPE) | Discipline (DISCIPLINE) | Document Code (DOCCODE) | Description |
|---|---|---|---|
| 275-CAL-001 | 275 | CAL | CALCULATION |
| 275-CON-001 | 275 | CON | CONTRACT |
| 275-CWP-001 | 275 | CWP | CONSTRUCTION WORK PACKAGE |
| 275-DBD-001 | 275 | DBD | DESIGN BASIS AND CRITERIA |
| 275-DBK-001 | 275 | DBK | PROJECT DATA BOOK |
| 275-DIA-001 | 275 | DIA | DIAGRAM |
| 275-DST-001 | 275 | DST | DATASHEET |
| 275-DTL-001 | 275 | DTL | DETAILS |
| 275-LAY-001 | 275 | LAY | LAYOUT |
| 275-LST-001 | 275 | LST | LIST |
| 275-RPT-001 | 275 | RPT | REPORT |
| 275-SPC-001 | 275 | SPC | SPECIFICATION |
| 275-STD-001 | 275 | STD | STANDARD |

### 500 – Construction

| Document Type (DOCTYPE) | Discipline (DISCIPLINE) | Document Code (DOCCODE) | Description                                              |
| ----------------------- | ----------------------- | ----------------------- | -------------------------------------------------------- |
| 500-CWP-001             | 500                     | CWP                     | CONSTRUCTION WORK PACKAGE                                |
| 500-DWG-001             | 500                     | DWG                     | ENGINEERED LIFT STUDY                                    |
| 500-EXE-001             | 500                     | EXE                     | CONSTRUCTION SCOPE OF WORK                               |
| 500-EXE-002             | 500                     | EXE                     | CONSTRUCTION EXECUTION PLAN                              |
| 500-EXE-003             | 500                     | EXE                     | MODULARIZATION AND FABRICATION PLAN                      |
| 500-FCN-001             | 500                     | FCN                     | FIELD CHANGE NOTICE                                      |
| 500-ITP-001             | 500                     | ITP                     | INSPECTION AND TEST PLAN                                 |
| 500-IWP-001             | 500                     | IWP                     | INSTALLATION WORK PACKAGE - ARCHITECTURAL                |
| 500-IWP-002             | 500                     | IWP                     | INSTALLATION WORK PACKAGE - CONCRETE FOUNDATIONS         |
| 500-IWP-003             | 500                     | IWP                     | INSTALLATION WORK PACKAGE - ELECTRICAL                   |
| 500-IWP-004             | 500                     | IWP                     | INSTALLATION WORK PACKAGE - FIREPROOFING                 |
| 500-IWP-005             | 500                     | IWP                     | INSTALLATION WORK PACKAGE - CIVIL                        |
| 500-IWP-006             | 500                     | IWP                     | INSTALLATION WORK PACKAGE - AUTOMATION HARDWARE          |
| 500-IWP-007             | 500                     | IWP                     | INSTALLATION WORK PACKAGE - CONTROL SYSTEMS              |
| 500-IWP-008             | 500                     | IWP                     | INSTALLATION WORK PACKAGE - PILING                       |
| 500-IWP-009             | 500                     | IWP                     | INSTALLATION WORK PACKAGE - MECHANICAL EQUIPMENT         |
| 500-IWP-010             | 500                     | IWP                     | INSTALLATION WORK PACKAGE - HVAC                         |
| 500-IWP-011             | 500                     | IWP                     | INSTALLATION WORK PACKAGE - PIPING                       |
| 500-IWP-012             | 500                     | IWP                     | INSTALLATION WORK PACKAGE - INSULATION                   |
| 500-IWP-013             | 500                     | IWP                     | INSTALLATION WORK PACKAGE - STRUCTURAL STEEL             |
| 500-IWP-014             | 500                     | IWP                     | INSTALLATION WORK PACKAGE - ELECTRICAL HEAT TRACING      |
| 500-IWP-015             | 500                     | IWP                     | INSTALLATION WORK PACKAGE - VESSEL LADDERS AND PLATFORMS |
| 500-JSA-001             | 500                     | JSA                     | JOB SAFETY ANALYSIS                                      |
| 500-RDL-001             | 500                     | RDL                     | REDLINE DRAWING                                          |
| 500-RPT-001             | 500                     | RPT                     | CONSTRUCTION SAFETY REPORT                               |
| 500-SKT-001             | 500                     | SKT                     | FIELD SKETCH                                             |
| 500-TVR-001             | 500                     | TVR                     | TURNOVER DOSSIER                                         |

### 653 – HSE, Fire Protection, LEED

| Document Type (DOCTYPE) | Discipline (DISCIPLINE) | Document Code (DOCCODE) | Description |
|---|---|---|---|
| 653-AUT-001 | 653 | AUT | AUTHORITY |
| 653-DBD-001 | 653 | DBD | DESIGN BASIS AND CRITERIA |
| 653-FHA-001 | 653 | FHA | FIRE HAZARD ANALYSIS |
| 653-LOP-001 | 653 | LOP | LOPA |
| 653-LST-001 | 653 | LST | LIST |
| 653-PHA-001 | 653 | PHA | PHA STUDY |
| 653-PHL-001 | 653 | PHL | PHILOSOPHY |
| 653-PLA-001 | 653 | PLN | PLAN |
| 653-PRC-001 | 653 | PRC | PROCEDURE |
| 653-QRA-001 | 653 | QRA | QUANTITATIVE RISK ASSESSMENT |
| 653-RPT-001 | 653 | RPT | REPORT |
| 653-SKT-001 | 653 | SKT | SKETCH |
| 653-SOW-001 | 653 | SOW | SCOPE OF WORK |
| 653-SPC-001 | 653 | SPC | SPECIFICATION |
| 653-TOR-001 | 653 | TOR | TERMS OF REFERENCE |

[^1]: **Open question:** The spec label reads "Leave as 00000" (5 zeros) but the format string shows `Y` (1 + 4 digits). The 8-character total (1 + 4 + 3 = 8) confirms 4 zeros is correct. The label text appears to be a spec discrepancy — not ours to correct.
[^2]: **Open question:** HVAC series 1000–1099 appears in all §4.2.x sequence tables and exceeds the 3-digit Sequence Number field. Resolution not defined in the reviewed specification.
[^3]: **Open question:** The spec example "LP100-DI-00000002, P&ID Lead Sheet 2" appears to be a full document number provided as context rather than the code value itself. The exact form of this segment requires clarification.
[^4]: **Open question:** The spec references "Sequence number from Section 4.1.4." Section 4.1.4 defines the Sector (N1) segment — not a P&ID sequence number. The intended reference is likely one of the §4.2.x sequence tables. Possible spec error — not ours to correct.
[^5]: **Open question:** The §4.6 format diagram marks the Sequence Number with "*see exception." This exception is not defined in the reviewed specification sections.
