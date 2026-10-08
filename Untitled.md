# Client Project Technical Document and Drafting Standard

**Document Number:** SCT.AIM.ST.3 **Revision:** 20 **Date:** Feb 5, 2026 **Document Owner:** AIM Supervisor **Document Focal:** Asset I&D Focal Point; Instr. I&D Focal Point; Asset & Projects I&D Specialist

---

## Table of Contents

1. [Introduction](#1-introduction)
2. [Client Technical Document Number Creation](#2-client-technical-document-number-creation)
3. [Client Technical Document Preparation](#3-client-technical-document-preparation)
4. [Client Technical Document and Data Storage](#4-client-technical-document-and-data-storage)
5. [Client Technical Document Revision Procedures](#5-client-technical-document-revision-procedures)
6. [Existing Client Technical Document Revision Procedures](#6-existing-client-technical-document-revision-procedures)
7. [As-Building](#7-as-building)
8. [Updating Non-Critical Documents](#8-updating-non-critical-documents)
9. [Vendor Documents](#9-vendor-documents)

---

## 1. Introduction

### 1.1 Purpose

This document's content is in accordance with the Client DEP 02.00.00.10-Gen Preparation of Technical Drawings requirements. It is intended for use by those creating new technical documents, changing technical documents for project execution, and those executing as-building and project close-out activities.

### 1.2 Intended Audience

EPCs and Client MOC PECs, Client TAO/Drafting team, Client Technical Library staff.

### 1.3 Definitions/Acronyms

#### 1.3.1 Acronyms/Abbreviations

|Acronym|Full Form|
|---|---|
|AIM|Asset Information Management|
|API|American Petroleum Institute|
|BOM|Bill of Materials|
|CCR|Continuous Catalytic Reformer|
|CO|Change Order|
|CWP|Construction Work Package|
|EHT|Electric Heat Tracing|
|EPC|Engineering, Procurement, Construction|
|IFC|Issued for Construction|
|IFR|Issued for Review|
|IFV|Issued for Void|
|LDT|Line Designation Table|
|MEG|Monoethylene Glycol|
|MOC|Management of Change|
|MRB|Manufacturer's Record Book|
|MTO|Material Take Off|
|NDE|Non-Destructive Examination|
|NHT|Naptha Hydrotreater|
|PEC|Person Executing Change|
|PDF|Portable Document Format|
|PDF/A|Portable Document Format (ISO-Standardized)|
|PDS|Plant Design Software|
|PFD|Process Flow Diagram|
|PRV|Pressure Relief Valve|
|P&ID|Process & Instrument Flow Diagram|
|QC|Quality Control|
|RV|Relief Valve|
|S3D|SmartPlant 3D|
|SPI|SmartPlant Instrumentation|
|SPP&ID|SmartPlant P&ID|
|SUP|Supersede|
|TAO|Technical Asset Operations|
|TDC|Technical Document Control|
|WPS|Welding Procedure Specification|

#### 1.3.2 Definitions

|Word|Definition|
|---|---|
|Client Critical Document|Any Client document that requires as-building|
|Client Master Document|Any Client document that functions as an original and is copied for use as an uncontrolled copy|
|Client Technical Document|Any Client document that is numbered according to the Client document numbering convention|
|AVEVA|The application that stores our Project asset tag data for all disciplines|

### 1.4 Functional Email Accounts

|Email|Purpose|
|---|---|
|SCAN-SCT-AIM@shell.com|Technical Document Numbering, Tag Management, TDN Support|
|CHN-RMZ-SCT-TAO-DC@shell.com|Projects Close Out Support|
|CHN-RMZ-SCT-TAO-EDR@shell.com|EDR Support|
|SCAN-SCT-MPG-TDC@shell.com|ASSAI SCT_MOD Support (IFD-IFC)|

### 1.5 Related Documents

1. Client DEP 02.00.00.10-Gen Preparation of Technical Drawings
2. Client DEP 01.00.09.10-Gen Tagging Specification and Symbols
3. ISO 15926 - Industrial Automation Systems and Integration
4. ISO 5455 - Technical Drawings - Scales
5. ISO 13567 - Technical Product Documentation - Organization and Naming of Layers for CAD

For standards, procedures, training materials and work instructions relating to SPI, SPP&ID and S3D, visit the AIM Forms, Procedures & Instructions SharePoint site and follow the headings for SmartPlant Instrumentation, SmartPlant P&ID, and 3D Design (PDS/S3D).

---

## 2. Client Technical Document Number Creation

### 2.1 What Belongs in the Technical Library?

The definition of technical information can help determine what belongs in the technical library or engineering application (SPI, SPPID, S3D) versus the MOC Project files. The term technical information refers to documents with asset or product related data and information that are used and stored for the purpose of:

1. Asset definition and specification
2. Asset design and engineering
3. Manufacturing and construction
4. Quality assurance
5. Describing the asset's functions and interfaces
6. Operating the asset (safe operating)
7. Maintaining the asset (asset integrity)
8. Installation of the asset
9. Changes to asset specifications
10. Documenting the state of the asset
11. Legal requirement
12. Future facility modifications

If the documentation does not fit the criteria above, it is likely a MOC project deliverable. For MOC Project deliverable document types and standards out of the Project Projects group, refer to the PG-009 Project Document Numbering Tool for guidance on naming conventions that would be uploaded to ASSAI SCT_MOD (this is not applicable for eMOC).

### 2.2 Client Technical Document Numbering Breakdown

||Unit|Class/Subclass|Tag|Document Type|Sequence Number|
|---|---|---|---|---|---|
|Refinery/Chemicals Document Numbering Format|AA|BBCC|DDD(D)|EEE|F|
|Example Value|21|11P-|005|053|1|
|Upgrader Document Numbering Format|AAA|BBCC(CCC)|DDD(D)|EEE|F|
|Example Value|411|03AI|005|054|1|

**UNIT:** AA/AAA is a two or three-digit number used to identify the unit (plant) for the document.

**CLASS/SUBCLASS:** Subclass can be up to a seven-character code used to identify the document's class and subclass. The first and second characters represent the discipline. The subsequent characters represent Equipment Function and/or Commodity type. When there is no 4th character, a hyphen "-" will be used. Refer to SCT.AIM.IDX.1 - Client Project Technical Document and Equipment Coding Index 'Class/Subclass' for the list of valid classes/subclasses. Note that each business has their own valid list of options; not all are accepted by all business areas.

**TAG:** DDD(D) is a three or four-digit number issued to identify the sequence of the specific tagged equipment (mechanical, electrical), line number or instrument loop number. When there is no specific tag associated with a document or there are multiple tags, the tag portion of the document number will be three zeros "000".

**DOCUMENT TYPE:** EEE is a three-character numeric code used to identify the type of document. Refer to SCT.AIM.IDX.1 'Document Type' tab for the list of valid document types.

**SEQUENCE NO#:** F begins as a single digit numeric code assigned by the Project AIM Department that provides a unique identifier to the document. As the number of drawings in the sequence increase, the F value will shift from single digits to double, triple, etc.

**Examples of Complete Document Numbers:**

1. Upgrader: 200.0000.000.041.1_V[#].dwg
2. Chemicals: 06.0000.000.041.1_V[#].dwg
3. Refinery: 24_0000_000_041_1_V[#].dwg (if a .cal file is also required, 24_0000_000_041_1_V[#].cal). Note: the document number as shown on a Refinery document shall have periods between the number sections (i.e. 24.0000.000.041.1), but the filename shall have underscores separating the number sections due to the Refinery and Chemical assets sharing the same unit numbers (i.e. 24_0000_000_041_1).

**Exceptions:**

1. Upgrader North is the only asset with EHT P&IDs in this format: UUU.1530.000.041 (some 2010 UPG South exist in PDF).
2. Bentley Nevada Master Trip Point Alarms Configuration should be coded under 1628 subclass. Refinery and Chemicals don't have these, but they are being met through the C&E documents. Upgrader has them.
3. Flow Compensation Calculations (CCF) exists in Upgrader in one document, but data is not consistent for Refinery and Chemicals. Should be coded under a 1612 subclass.
4. Fireproofing Zone Plot Plans should be Document type 044. These only exist for units 221, 211, 30, 22, 12 and 440.

### 2.3 How to Request a Change to the Document Numbering Categories

There are specific codes used to develop Client technical document numbers. Care must be taken to maintain a consistent numbering system which might require the addition/deletion or updating of codes. Before requesting a new or a change to a code, consider:

1. Will the coding change impact other documents?
2. Does the coding change follow the logic in the coding manual?
3. Could a new code potentially be misinterpreted? Does it represent another code type or tag in the facility?

To request a change to document code (unit, class, subclass, or document type), contact the AIM Supervisor. The AIM Supervisor will ensure the request is valid, obtain approval, and ensure the new code is added/deleted/updated to all applicable databases.

### 2.4 Client eMOC Checklist

All technical documents that will reside in ASSAI SCT_OPS, S3D and SPP&ID shall be assigned a Client technical document number. The Client eMOC Checklist (SUG.CON.MOC.F.002 MOC Closeout Checklist) details the technical document deliverables for each discipline, their criticality and where they are stored. Use this document to aid in identifying which document types shall be delivered to the Client AIM department for filing.

### 2.5 Generating a New Client Technical Document Number

All new (or existing) Client technical documents that will be/are filed in ASSAI SCT_OPS, S3D or SPP&ID shall be assigned a Client technical document number (see notes 1-4). Refer to SCT.AIM.IDX.1 for a list of Units, Classes and Document Types used at Project. Requests for new Client technical document numbers will be sent to the Project AIM Team using AVEVA Work Task (see SCT.AIM.WI.9 for training).

All new document numbers are generated in AVEVA Work Task and stored in ASSAI SCT_OPS for all Project businesses (Upgrader, Refinery and Chemicals). Any unused, new Client technical document number shall be cancelled during or at the end of the project by returning the SCT.AIM.F.1 routing form with the "Cancellation of Placeholder" tab filled out. To align with DEP 02.00.00.10-Gen Section 4.1.4, "document numbers of cancelled drawings or documents shall not be re-used"; the Client Technical Document Number will be de-activated and not deleted.

**Note 1:** This does not apply to Sketches (see Sketch Section 3.4.2.1).

**Note 2:** Documents or datasheets housed in SPI do not require a Client technical document number; they receive their own numbers through the SPI application.

**Note 3:** Loop/Wiring instrument documents for Manufacturing are housed in ASSAI SCT_OPS and do require a Client technical document number.

**Note 4:** Existing Braun or Badger documents (see Section 2.8) shall be assigned a Client technical document number upon being as-built. They shall continue to possess the old historical document number for referencing purposes.

**Note 5:** All new Client technical document filenames shall follow this standard: [TECHNICAL DOCUMENT NUMBER]_V[#].[FILETYPE].

**Note 6:** Document numbers shall be consistent and stable throughout the life of the document.

### 2.6 Client Technical Documents that Apply to Multiple Units

Some documents may apply to multiple units at Project. The following rules apply for selecting the appropriate unit for a document's number and metadata.

Within ASSAI, there are four common units: Unit 00, Unit 06, Unit 200 & Unit 400. There are also common units within the Process Units.

**Common Unit 00 shall be used when:**

1. The document references 2 or more equipment numbers in different units within the Refinery facility that are not part of the same process unit.
2. The document references two or more equipment numbers from Refinery, Chemicals and/or Upgrader Units.

**Common Unit 06 shall be used when:**

1. The document references 2 or more equipment numbers in different units within the Chemicals facility that are not part of the same process unit.

**Common Unit 200 shall be used when:**

1. The document references two or more equipment numbers in different units within the 200 series (base plant Upgrader) that are not part of the same process unit.
2. The document references two or more equipment numbers from both the 200 and 400 series (base and expansion Upgrader).

**Common Unit 400 shall be used when:**

1. The document references 2 or more equipment numbers in different units within the 400 series (expansion Upgrader) that are not part of the same process unit.

**Process unit "Common Units" shall be used when:**

1. The document references 2 or more equipment numbers in different units within the same Process Unit. Examples: C-21501 & C-21601 use Unit 217; MS-3101 & MS-3201 use Unit 30 (MEG); C-3101 & C-3201 use Unit 30 (NHT/CCR); E-4101 & E-4301 use Unit 40 (Aromatics Common).

**Exception:** When a document references 2 or more equipment numbers within the same process unit and they are in twin trains, the Train 1 Unit number shall be used. Example: V-24101 & V-24201 use Unit 241. Example: E-2201 & E-2301 use Unit 22.

### 2.7 Client Technical Documents that Apply to Multiple Tags

Client technical document numbers are designed to help users identify what asset tag the document pertains to. When you have 1 tag the document highlights, you shall create a Client technical document number from which the tag can be derived. Example: an isometric for SS-22001 yields document number 22_03SS_001_054. Another example: an isometric for Badger line # 8676 yields [Unit line is in].0308.676.054.

For documents pertaining to multiple tags:

1. P&ID = 000
2. Document with piping and EHT on it = 000
3. MRB for twinned/tripled/quadrupled equipment: one document shall represent all assets that are identical in make, model, design, etc. Example: V-2302A and V-2302B MRB will be one document numbered 23_08V-_02-_025.
4. Equipment datasheets for twinned equipment: one datasheet shall represent all identical assets. Example: P-2301A and P-2301B will be one datasheet numbered 23_11P-_01-_035.
5. If the document pertains to more than one asset of different tag sequences or equipment types (e.g. P-23001, SS-23002), the tag portion shall be 000 with a generalized subclass code.

### 2.8 Client Technical Documents that Have Multiple Sheets

Requirements for multi-sheet documents:

1. The document shall indicate the sheet number out of total sheets (e.g. Sheet 1 of 4). The sheet number shall be in the title block, not part of the document number.
2. Each sheet of a multi-sheet drawing shall be stored as a separate file.
3. Each numbered sheet shall have its own revision code.
4. The document filename shall follow: [Client Technical Document Number] Sheet [# of #]_V[#].dwg.
5. When entering the document into ASSAI, the 'Sheet Nr' field shall be filled in (e.g. "1/2", "2/2").
6. Multi-sheet technical documents shall have a cover sheet with the document number in the title block.
7. The technical document number shall be repeated on all sheets.
8. Index sheets shall indicate at minimum the revision status of each sheet and division blocks of sheet numbers (if applicable).

### 2.9 Client Technical Documents with Appendixes

Some technical documents will have appendixes that need to be editable for future change. Requirements:

1. The technical document must indicate under each Appendix title that there is an editable version located in the technical library.
2. File shall be embedded into that technical document's revision. Filename of the appendix should match the technical document number (e.g. 272.0008.000.026.001_appendix.xls). The appendices will be stored underneath the published technical document file in the technical library.

---

## 3. Client Technical Document Preparation

### 3.1 Computer Aided Drafting (CAD)

#### 3.1.1 CAD Software

The CAD software used to produce drawings shall be approved by Client Project. Currently, the Project facility uses:

1. AutoCAD 2019 or AutoCAD 2021
2. Microstation Connect Edition Update 13
3. AutoDesk Raster Design 2019 or AutoDesk Raster Design 2021

#### 3.1.2 Exchange Format

Unless prior approval is received from Client, all new drawings shall be prepared using AutoCAD with monochrome CTB and saved in AutoCAD 2010 version compatibility: Save As - "AutoCAD 2010/LT 2010 Drawing (*.dwg)". Drawings prepared using other CAD programs shall be transferred into AutoCAD format prior to turnover (excluding drawings from PDS/S3D model and Microstation). When conversions must be made, basic graphic entities such as lines, arcs, ellipses, blocks and text strings shall be preserved. If an intelligent/3D CAD application is used, the system shall conform to ISO 15926 to enable exchange of data to alternative CAD applications.

#### 3.1.3 Hard Copy Drawings

All hard copy drawings (critical and non-critical) shall be scanned to create an electronic file. The 'raster' file will be coupled with an AutoCAD drawing template to form a hybrid (compound) drawing, which becomes the new drawing format. AutoCAD Raster Design 2009 is the required software to manage hybrid drawings. Both files (CAL and DWG) must have identical filenames and together create the compound document. In case of a poor-quality image, the drawing or part of the drawing shall be redrawn.

### 3.2 Microstation

There is currently no standard Client Project format for Microstation drawings. The same format shall be adhered to within a Microstation drawing when revising it. For new drawings where similar existing drawings were created in Microstation, the new drawings shall adhere to the same format. Microstation files shall not be converted to AutoCAD.

### 3.3 Printing and Plotting

The official plotted version of a technical drawing shall have the physical dimensions specified in Section 3.5, with no impact to legibility.

### 3.4 Templates

#### 3.4.1 Critical Client Technical Document Templates

1. The Client critical document list can be found in the SUG.CON.MOC.F.002 MOC Closeout Checklist. They are marked with an X in column B and indicated as stored in ASSAI SCT_OPS/SPI/SPPID/S3D/SharePoint RV Library. Note: data stored in SPI or SharePoint RV Library do not have Client Technical Document Numbers applied.
2. Client Project has developed standard templates located in the AIM Forms SharePoint site under Drafting & Design - Templates - SCT.AIM.TMP.4, for use when creating new critical Client technical documents (AutoCAD, Excel, Word).
3. Some critical Client technical documents will be created outside of AutoCAD/Excel/Word (e.g. instrument datasheets, some P&IDs, isometrics). Reference Section 3.0 and Section 1.5 for those exceptions and procedures.
4. If creating a new P&ID AutoCAD document, a 'P&ID Change List' shall also be created; all other process deliverables do not require a change list.
5. If creating a new Process Flow Diagram, it shall be a multi-sheet drawing with an index containing document number, title and revision. All sheets must be individual files, not a CAD drawing with multiple sheets set up as tabs.
6. All new critical Client technical documents shall have a Client technical document number assigned before being issued via a project transmittal (see Section 2.0).

#### 3.4.2 Non-Critical Client Technical Document Templates

1. Client non-critical document list can be found in SUG.CON.MOC.F.002 MOC Closeout Checklist. They are not marked with an X in column B but are indicated as stored in ASSAI SCT_OPS.
2. Client Project has developed standard templates for critical Client technical documents (in the AIM Forms SharePoint site under Drafting & Design - Templates - SCT.AIM.TMP.4) that may also be used when creating non-critical documents.
3. There are additional non-critical documents that could be generated as part of Project work (e.g. bill of materials, installation detail, sketch, MTO, tie point schedules, photos). Client Project does not have templates for these; they are at their creators' discretion. However, there is a go-by document for MTO (see Appendix A).

##### 3.4.2.1 Sketches

Sketches are documents generated during project execution that are not intended to be retained within Client technical document repositories once the project is completed.

1. Sketch numbers are for documents containing information only relevant for the project, with no further use once completed.
2. A sketch shall never be uploaded to Client technical document repositories such as ASSAI SCT_OPS, SPI, SPP&ID.
3. Any document put in the technical repositories is not a sketch and shall be assigned a Client technical document number before being Issued for Construction (see Section 2.4).
4. Documents that end up in technical repositories (and therefore are not sketches) include: Client critical documents or traditionally as-built documents, and documents of a technical nature expected to be found in a technical library after a project (isometrics, plans, elevations, details, schematics, loop diagrams, contour maps, etc.).
5. Good examples of sketches: photos with or without markups, model shots, "for information" documents not stamped or to be relied upon.
6. For sketch numbering see the PG-009 Project Document Numbering Tool. The EPC controls the sequence numbers of sketches and does not request sketch numbers from Client TDC.
7. Documents that were traditionally given sketch numbers have now been given naming standards under PG-009.
8. A sketch shall not be used to merge changes into master files. Critical Client technical documents such as LDTs and electrical schedules that the project uses a template for during design will be incorporated into the Client master critical document at close-out.

### 3.5 Drawing Sizes

Standard metric sheet sizes for new electronic or rasterized drawings:

|Size No.|Sheet Size (mm)|Borders (mm)|
|---|---|---|
|A1|841 x 594|10|
|A2|594 x 420|10|
|A3|420 x 297|5|
|A4|210 x 297|5|

For scaled drawings, the sheet size should be multiplied by the scale factor to obtain the electronic drawing limit values. Drawings shall be composed so that a reduced A3 plot size is clear and legible. Drawing content shall be spaced out to prevent crowding or overlapping of views and text. Details shall be organized so related information reads coherently in a grouped arrangement.

### 3.6 Layout

#### 3.6.1 General

1. Drawings shall be composed so that a reduced A3 plot size is clear and legible.
2. Drawing content shall be spaced out to prevent crowding or overlapping.
3. Details shall be organized so related information reads coherently in a grouped arrangement.

#### 3.6.2 Title Block

For all CAD documents within the technical libraries, the title block shall be shown in the right-hand bottom corner. Drawing titles shall not be abbreviated and include the following in this order:

1. 'Area - Unit - Unit description' or, if not specific to a Unit, then 'Area - Description'.
2. 'Equipment Tag' and 'Description/Service of Equipment' (if applicable) or 'Class/Subclass' if not applicable to a specific piece of equipment.
3. 'Document Type'.

**Note:** There are no requirements for title block for text documents.

**Note:** Documents developed during the original construction of the Refinery or Chemicals assets possess a historical project-related number that shall remain on the document. Examples:

1. **Original Braun Document Number (Refinery Only):** When Refinery was constructed in 1984 by Braun, the original documents were turned over with Braun's document codes instead of Client technical document numbers (e.g. 9018-130-CD-100 or 9018-100-400-3). Anything created after this does not have Braun document numbers.
2. **Original Badger Document Number (Chemicals Only):** When Chemicals was constructed in 1986 by Badger, the original documents were turned over with Badger's document codes (e.g. E7921-1509-H-28 or SPE-7921-C-1). Anything created after this does not have Badger document numbers.

**AutoCAD:** Document titles are created using Title 1, Title 2, Title 3 and Title 4. Each title represents a new line in the title block; not all titles use 4 lines.

Example for 20.0000.000.041.49:

- Title 1: Distillate Hydrogenation Treater - Unit 20
- Title 2: Flare K.O. Drum & Pumps
- Title 3: V-2023, P-2014A/B
- Title 4: Piping and Instrument Flow Diagram

Example for 26.1514.000.065.10:

- Title 1: Hydrogen Compression Facility - Unit 26
- Title 2: Area - All Electrical
- Title 3: Panel 26-UP-A & 26-DCP-A
- Title 4: Cable and Conduit Schedule

Example for 25.11P-.03A.077.1:

- Title 1: Distillate Hydrogenation Unit - Unit 25
- Title 2: P-2503A Light & Heavy Gas Oil
- Title 3: General Arrangement

**Excel:** Example for 01.1514.000.065.902:

- Title 1: Ethyl Benzene - Unit 01
- Title 2: EHT Power, Control & Communication
- Title 3: Cable Schedule
- Title 4: Dwg No.
- Title 5: 01.1514.000.065.902

**Word or PDF:** If the PDF is an AutoCAD drawing, follow the AutoCAD title block section. Otherwise, include: Document Number - Equipment Tag Description of Service. Example: 211.11C-.01-.021.1 - C-21101 Compressor Installation, Operation and Maintenance Manual.

#### 3.6.3 Client Legal Name

Client Project has two different legal names. This name shall be present on the Client technical document for the appropriate asset in the title block. If the name is incorrect on an existing document, do not change:

1. Refinery and Chemicals drawings/documents: Client Canada Products
2. Upgrader drawings/documents: Client Canada Energy

#### 3.6.4 Scale

On all drawings other than schematics/diagrams or A4 sheet size, a figured scale bar at least 100mm (4 inches) long shall be added to indicate the original scale. Scales shall conform to ISO 5455. The scale shall be noted beneath each view if different from the overall drawing scale.

#### 3.6.5 Orientation

1. Layout drawings should be oriented with Plant North pointing towards the top of the drawing sheet. Plant North may point to the left of the sheet if it enables better use of the sheet.
2. Plan drawings should be oriented with each sheet indicating North in the same direction.
3. The arrow indicating Plant North shall be positioned in the top left-hand corner of the drawing.
4. For plot plans and topographical drawings, a combined symbol for True North, Plant North and prevailing wind shall be used.

### 3.7 Lettering

#### 3.7.1 Document Number

Minimum text height of the drawing document number in the title block:

|Size|A1|A2|A3|A4|
|---|---|---|---|---|
|Minimum Height (mm)|4.5|3|2.5|2.5|

#### 3.7.2 Textual Information

1. All text shall be in the English language.
2. Minimum height of text and figures for A1-A4 sizes: 2.5mm.
3. The CAD text font shall be based on a True Type font. Microstation only: the font titled "working" shall not be used, as this text is not recognized by the Digital Twin.
4. The width to height ratio of the font shall be 1:1.
5. All lettering shall be uppercase except for units of measure abbreviations.
6. Abbreviations applied on drawings shall be limited to those approved by the project.

### 3.8 Line Thicknesses

|Size of Drawing|A1|A2, A3 and A4|
|---|---|---|
|Thick Lines|0.7mm|0.35mm|
|Medium Lines|0.5mm|0.35mm|
|Narrow Lines (Including Dimensions, Text)|0.35mm|0.25mm|

### 3.9 Layers

#### 3.9.1 Convention

Layer naming and usage shall be in accordance with ISO 13567.

#### 3.9.2 Usage of Layers

1. Layers should only be applied to support a drafting function.
2. Layering shall not be used to save more than one registered document per drawing file.
3. The drawing template, including the title block, shall be drawn on a separate layer.
4. To standardize presentation and plotting of electronic drawings, a layering structure has been developed for each category of drawing, stored as ".dwg" blocks. The appropriate layer block shall be inserted into the standard drawing sheet block for each new drawing.
5. Additional layers, depending on specific needs, will be discussed and approved by the Client Project AIM department.

|Block Name (.dwg)|Layer Description|
|---|---|
|PIDLAYER.dwg|Layer Defaults for P&ID|
|ISOLAYER.dwg|Layer Defaults for Piping Isometrics|
|ORTHLAYR.dwg|Layer Defaults for Piping Plans|
|EHTLAYER.dwg|Layer Defaults for Electric Heat Tracing Isometrics|
|ELINLAYER.dwg|Layer Defaults for Electrical and Instrumentation|
|CIVLAYER.dwg|Layer Defaults for Civil Drawings|
|STRLAYER.dwg|Layer Defaults for Structural Drawings|
|UGLAYER.dwg|Layer Defaults for Underground Drawings|

#### 3.9.3 Layer Defaults

##### Piping and Instrumentation Diagrams (P&IDs)

|Name|Color|Linetype|Lineweight|
|---|---|---|---|
|0|white|CONTINUOUS|ByLineWeightDefault|
|ATEXT|yellow|CONTINUOUS|ByLineWeightDefault|
|BORDER|11|CONTINUOUS|ByLineWeightDefault|
|BOUNDARY|134|PHANTOM|ByLineWeightDefault|
|CENTER|yellow|CENTER|ByLineWeightDefault|
|CLOUD|150|CONTINUOUS|ByLineWeightDefault|
|CONST|white|CONTINUOUS|ByLineWeightDefault|
|CPLP|white|CONTINUOUS|ByLineWeightDefault|
|CPRT|white|CONTINUOUS|ByLineWeightDefault|
|DIMN|green|CONTINUOUS|ByLineWeightDefault|
|EQUIP|9|CONTINUOUS|ByLineWeightDefault|
|FITTING|red|CONTINUOUS|ByLineWeightDefault|
|INSTBALLOON|yellow|CONTINUOUS|ByLineWeightDefault|
|INSTLINECAP|130|CONTINUOUS|ByLineWeightDefault|
|INSTLINEHYD|130|CONTINUOUS|ByLineWeightDefault|
|INSTLINELEC|130|DASHED|ByLineWeightDefault|
|INSTLINEMAG|130|CONTINUOUS|ByLineWeightDefault|
|INSTLINEMIC|130|CONTINUOUS|ByLineWeightDefault|
|INSTLINEPN|130|CONTINUOUS|ByLineWeightDefault|
|INSTVL|130|CONTINUOUS|ByLineWeightDefault|
|LOCK|60|CONTINUOUS|ByLineWeightDefault|
|MANVL|130|CONTINUOUS|ByLineWeightDefault|
|MATCHLINE|11|CONTINUOUS|ByLineWeightDefault|
|MEDFLOW|red|CONTINUOUS|ByLineWeightDefault|
|SYMBOL|130|CONTINUOUS|ByLineWeightDefault|
|TEXT|yellow|CONTINUOUS|ByLineWeightDefault|
|THKFLOW|magenta|CONTINUOUS|ByLineWeightDefault|
|THNFLOW|130|CONTINUOUS|ByLineWeightDefault|
|TRACER|134|DASHED|ByLineWeightDefault|
|TTEXT|9|CONTINUOUS|ByLineWeightDefault|

The layer structure is saved as a block and inserted into P&ID drawing sheets from PIDLAYER.dwg (Insertion point 0,0). This layering system is based on the Client version of CADpipe P&ID. Any additional layers required beyond those listed must receive prior approval from Client AIM.

##### Piping Isometrics

|Name|Color|Linetype|Lineweight|
|---|---|---|---|
|0|white|CONTINUOUS|ByLineWeightDefault|
|BALLOON|red|CONTINUOUS|ByLineWeightDefault|
|BORDER|11|CONTINUOUS|ByLineWeightDefault|
|CENTER|yellow|CPCENTER|ByLineWeightDefault|
|CLOUD|150|CONTINUOUS|ByLineWeightDefault|
|CPLP|white|CONTINUOUS|ByLineWeightDefault|
|CPRT|white|CONTINUOUS|ByLineWeightDefault|
|DIMN|green|CONTINUOUS|ByLineWeightDefault|
|EQUIP|9|CONTINUOUS|ByLineWeightDefault|
|EXIST|green|DASHED|ByLineWeightDefault|
|FITG|red|CONTINUOUS|ByLineWeightDefault|
|LEADER|red|CONTINUOUS|ByLineWeightDefault|
|PIPE|magenta|CONTINUOUS|ByLineWeightDefault|
|SYMBOL|yellow|CONTINUOUS|ByLineWeightDefault|
|TEXT|yellow|CONTINUOUS|ByLineWeightDefault|
|TITLE|red|CONTINUOUS|ByLineWeightDefault|
|TTEXT|9|CONTINUOUS|ByLineWeightDefault|
|WELD|red|CONTINUOUS|ByLineWeightDefault|

Inserted from ISOLAYER.dwg (Insertion point 0,0). Based on the CADpipe ISO prototype drawing. Any additional layers require prior approval from Client AIM.

##### Piping Plans

|Name|Color|Linetype|Lineweight|
|---|---|---|---|
|0|white|CONTINUOUS|ByLineWeightDefault|
|BORDER|11|CONTINUOUS|ByLineWeightDefault|
|CENTER|yellow|CENTER|ByLineWeightDefault|
|CLOUD|150|CONTINUOUS|ByLineWeightDefault|
|CONST|white|CONTINUOUS|ByLineWeightDefault|
|CP3D|magenta|CONTINUOUS|ByLineWeightDefault|
|CPISO|cyan|CONTINUOUS|ByLineWeightDefault|
|CPLP|white|CONTINUOUS|ByLineWeightDefault|
|CPRT|white|CONTINUOUS|ByLineWeightDefault|
|DIMN|green|CONTINUOUS|ByLineWeightDefault|
|EQUIP|9|CONTINUOUS|ByLineWeightDefault|
|EXIST1|green|DASHED|ByLineWeightDefault|
|EXIST2|green|DASHED|ByLineWeightDefault|
|FITG1|magenta|CONTINUOUS|ByLineWeightDefault|
|FITG2|red|CONTINUOUS|ByLineWeightDefault|
|GASKET|white|CONTINUOUS|ByLineWeightDefault|
|MATCHLINE|11|CONTINUOUS|ByLineWeightDefault|
|PIPE1|magenta|CONTINUOUS|ByLineWeightDefault|
|PIPE2|red|CONTINUOUS|ByLineWeightDefault|
|PLANHIDE|130|CONTINUOUS|ByLineWeightDefault|
|SECT1E|green|HIDDEN|ByLineWeightDefault|
|SECT1F|green|CONTINUOUS|ByLineWeightDefault|
|SECT1P|green|CONTINUOUS|ByLineWeightDefault|
|SECT2E|green|HIDDEN|ByLineWeightDefault|
|SECT2F|green|CONTINUOUS|ByLineWeightDefault|
|SECT2P|green|CONTINUOUS|ByLineWeightDefault|
|SYMBOL|yellow|CONTINUOUS|ByLineWeightDefault|
|TEXT|yellow|CONTINUOUS|ByLineWeightDefault|
|TITLE|red|CONTINUOUS|ByLineWeightDefault|
|TTEXT|9|CONTINUOUS|ByLineWeightDefault|
|WELD|red|CONTINUOUS|ByLineWeightDefault|

Inserted from ORTHLAYR.dwg. Plant coordinate system is often used. Based on the CADpipe ORTHO prototype drawing. Any additional layers require prior approval from Client AIM.

##### Electric Heat Tracing Isometrics

|Name|Color|Linetype|Lineweight|
|---|---|---|---|
|0|white|CONTINUOUS|ByLineWeightDefault|
|BALLOON|red|CONTINUOUS|ByLineWeightDefault|
|BORDER|11|CONTINUOUS|ByLineWeightDefault|
|CENTER|yellow|CONTINUOUS|ByLineWeightDefault|
|CLOUD|150|CONTINUOUS|ByLineWeightDefault|
|CPLP|white|CONTINUOUS|ByLineWeightDefault|
|CPRT|white|CONTINUOUS|ByLineWeightDefault|
|DIMN|green|CONTINUOUS|ByLineWeightDefault|
|EQUIP|9|CONTINUOUS|ByLineWeightDefault|
|EXIST|green|DASHED|ByLineWeightDefault|
|FITG|red|CONTINUOUS|ByLineWeightDefault|
|LEADER|red|CONTINUOUS|ByLineWeightDefault|
|LOCK|60|CONTINUOUS|ByLineWeightDefault|
|PIPE|red|CONTINUOUS|ByLineWeightDefault|
|SECTOR|green|CONTINUOUS|ByLineWeightDefault|
|SYMBOL|60|CONTINUOUS|ByLineWeightDefault|
|TEXT|yellow|CONTINUOUS|ByLineWeightDefault|
|TITLE|red|CONTINUOUS|ByLineWeightDefault|
|TRACER|magenta|DASHED|ByLineWeightDefault|
|TTEXT|9|CONTINUOUS|ByLineWeightDefault|
|WELD|red|CONTINUOUS|ByLineWeightDefault|

Inserted from EHTLAYER.dwg (Insertion point 0,0). Based on the CADpipe ISO prototype drawing. Any additional layers require prior approval from Client AIM.

##### Electrical and Instrumentation

|Name|Color|Linetype|Lineweight|
|---|---|---|---|
|0|white|CONTINUOUS|ByLineWeightDefault|
|ATEXT|yellow|CONTINUOUS|ByLineWeightDefault|
|BORDER|11|CONTINUOUS|ByLineWeightDefault|
|BOUNDARY|134|PHANTOM|ByLineWeightDefault|
|BUS|magenta|CONTINUOUS|ByLineWeightDefault|
|CABLETRAY|221|CONTINUOUS|ByLineWeightDefault|
|CENTER|yellow|CENTER|ByLineWeightDefault|
|CLASSAREA|221|CONTINUOUS|ByLineWeightDefault|
|CLOUD|150|CONTINUOUS|ByLineWeightDefault|
|CONDUIT|131|CONTINUOUS|ByLineWeightDefault|
|CONST|white|CONTINUOUS|ByLineWeightDefault|
|DIMN|green|CONTINUOUS|ByLineWeightDefault|
|EQUIP|9|CONTINUOUS|ByLineWeightDefault|
|EXIST|green|DASHED|ByLineWeightDefault|
|FWIRE|red|DASHED|ByLineWeightDefault|
|GRDWIRE1|red|CONTINUOUS|ByLineWeightDefault|
|GRDWIRE2|red|DASHED|ByLineWeightDefault|
|INSTLINE1|131|CONTINUOUS|ByLineWeightDefault|
|INSTLINE2|131|DASHED|ByLineWeightDefault|
|INSTLOOP|60|CONTINUOUS|ByLineWeightDefault|
|LOCK|60|CONTINUOUS|ByLineWeightDefault|
|MATCHLINE|11|PHANTOM|ByLineWeightDefault|
|PIPE|red|CONTINUOUS|ByLineWeightDefault|
|SECTOR|green|CONTINUOUS|ByLineWeightDefault|
|SYMBOL|60|CONTINUOUS|ByLineWeightDefault|
|TERMSTRIP|red|CONTINUOUS|ByLineWeightDefault|
|TEXT|yellow|CONTINUOUS|ByLineWeightDefault|
|TITLE|red|CONTINUOUS|ByLineWeightDefault|
|TRACER|magenta|DASHED|ByLineWeightDefault|
|TTEXT|9|CONTINUOUS|ByLineWeightDefault|
|UGRDCOND|131|DASHED|ByLineWeightDefault|
|WIRE|red|CONTINUOUS|ByLineWeightDefault|

Inserted from ELINLAYR.dwg (Insertion point 0,0). Any additional layers require prior approval from Client AIM.

##### Civil Drawings

|Name|Color|Linetype|Lineweight|
|---|---|---|---|
|0|white|CONTINUOUS|ByLineWeightDefault|
|ATEXT|yellow|CONTINUOUS|ByLineWeightDefault|
|BORDER|11|CONTINUOUS|ByLineWeightDefault|
|BOUNDARY|134|CONTINUOUS|ByLineWeightDefault|
|CENTER|yellow|CENTER|ByLineWeightDefault|
|CLOUD|150|CONTINUOUS|ByLineWeightDefault|
|CONCRETE1|cyan|CONTINUOUS|ByLineWeightDefault|
|CONCRETE2|134|CONTINUOUS|ByLineWeightDefault|
|CONCRETE3|134|DASHED|ByLineWeightDefault|
|CONST|white|CONTINUOUS|ByLineWeightDefault|
|DIMN|green|CONTINUOUS|ByLineWeightDefault|
|EQUIP|9|CONTINUOUS|ByLineWeightDefault|
|GRADE|14|CONTINUOUS|ByLineWeightDefault|
|GRATING|130|CONTINUOUS|ByLineWeightDefault|
|HATCH1|cyan|CONTINUOUS|ByLineWeightDefault|
|HATCH2|white|CONTINUOUS|ByLineWeightDefault|
|MATCHLINE|11|PHANTOM|ByLineWeightDefault|
|PILE1|15|CONTINUOUS|ByLineWeightDefault|
|PILE2|15|DASHED|ByLineWeightDefault|
|REBAR1|10|CONTINUOUS|ByLineWeightDefault|
|REBAR2|221|CONTINUOUS|ByLineWeightDefault|
|REBAR3|221|DASHED|ByLineWeightDefault|
|SECTION|yellow|CONTINUOUS|ByLineWeightDefault|
|STEEL4|13|CONTINUOUS|ByLineWeightDefault|
|STEEL5|13|DASHED|ByLineWeightDefault|
|SYMBOL|yellow|CONTINUOUS|ByLineWeightDefault|
|TEXT|yellow|CONTINUOUS|ByLineWeightDefault|
|TITLE|red|CONTINUOUS|ByLineWeightDefault|
|TTEXT|9|CONTINUOUS|ByLineWeightDefault|
|WELD|red|CONTINUOUS|ByLineWeightDefault|

Inserted from CIVLAYR.dwg. Plant coordinate system is often used. Any additional layers require prior approval from Client AIM.

##### Structural Drawings

|Name|Color|Linetype|Lineweight|
|---|---|---|---|
|0|white|CONTINUOUS|ByLineWeightDefault|
|ATEXT|yellow|CONTINUOUS|ByLineWeightDefault|
|BORDER|11|CONTINUOUS|ByLineWeightDefault|
|BOUNDARY|134|CONTINUOUS|ByLineWeightDefault|
|CENTER|yellow|CENTER|ByLineWeightDefault|
|CLOUD|150|CONTINUOUS|ByLineWeightDefault|
|CONCRETE4|221|CONTINUOUS|ByLineWeightDefault|
|CONCRETE5|221|PHANTOM|ByLineWeightDefault|
|CONST|white|CONTINUOUS|ByLineWeightDefault|
|DIMN|green|CONTINUOUS|ByLineWeightDefault|
|EQUIP|9|CONTINUOUS|ByLineWeightDefault|
|GRATING|130|CONTINUOUS|ByLineWeightDefault|
|HATCH1|cyan|CONTINUOUS|ByLineWeightDefault|
|HATCH2|white|CONTINUOUS|ByLineWeightDefault|
|MATCHLINE|11|PHANTOM|ByLineWeightDefault|
|SECTION|yellow|CONTINUOUS|ByLineWeightDefault|
|STEEL1|10|CONTINUOUS|ByLineWeightDefault|
|STEEL2|130|CONTINUOUS|ByLineWeightDefault|
|STEEL3|130|PHANTOM|ByLineWeightDefault|
|SYMBOL|yellow|CONTINUOUS|ByLineWeightDefault|
|TEXT|yellow|CONTINUOUS|ByLineWeightDefault|
|TITLE|red|CONTINUOUS|ByLineWeightDefault|
|TTEXT|9|CONTINUOUS|ByLineWeightDefault|
|WELD|red|CONTINUOUS|ByLineWeightDefault|

Inserted from STRLAYER.dwg (Insertion point 0,0). Any additional layers require prior approval from Client AIM.

##### Underground Drawings

|Name|Color|Linetype|Lineweight|
|---|---|---|---|
|0|white|CONTINUOUS|ByLineWeightDefault|
|AI|cyan|CONTINUOUS|ByLineWeightDefault|
|ATEXT|yellow|CONTINUOUS|ByLineWeightDefault|
|AU|10|CONTINUOUS|ByLineWeightDefault|
|BORDER|11|CONTINUOUS|ByLineWeightDefault|
|BOUNDARY|134|PHANTOM|ByLineWeightDefault|
|BUILDING|9|CONTINUOUS|ByLineWeightDefault|
|CATHODIC|60|CONTINUOUS|ByLineWeightDefault|
|CB|130|CONTINUOUS|ByLineWeightDefault|
|CENTER|yellow|CENTER|ByLineWeightDefault|
|CLOUD|150|CONTINUOUS|ByLineWeightDefault|
|CONCRETE|white|CONTINUOUS|ByLineWeightDefault|
|CONDUIT|131|CONTINUOUS|ByLineWeightDefault|
|CONST|white|CONTINUOUS|ByLineWeightDefault|
|DATA|130|CONTINUOUS|ByLineWeightDefault|
|DB|magenta|CONTINUOUS|ByLineWeightDefault|
|DIMN|green|CONTINUOUS|ByLineWeightDefault|
|DM|11|CONTINUOUS|ByLineWeightDefault|
|DR|11|CONTINUOUS|ByLineWeightDefault|
|DRC|150|CONTINUOUS|ByLineWeightDefault|
|DS|11|CONTINUOUS|ByLineWeightDefault|
|DSU|magenta|CONTINUOUS|ByLineWeightDefault|
|DUCT|red|CONTINUOUS|ByLineWeightDefault|
|EF|cyan|CONTINUOUS|ByLineWeightDefault|
|EQUIP|9|CONTINUOUS|ByLineWeightDefault|
|FENCE|221|CONTINUOUS|ByLineWeightDefault|
|FIBER|131|CONTINUOUS|ByLineWeightDefault|
|FITG|red|CONTINUOUS|ByLineWeightDefault|
|FOUND|12|CONTINUOUS|ByLineWeightDefault|
|GN|cyan|CONTINUOUS|ByLineWeightDefault|
|GRADELINE|13|CONTINUOUS|ByLineWeightDefault|
|GRID|white|CONTINUOUS|ByLineWeightDefault|
|GROUND|red|CONTINUOUS|ByLineWeightDefault|
|HIGHVOLT|8|CONTINUOUS|ByLineWeightDefault|
|HYDRANT|221|CONTINUOUS|ByLineWeightDefault|
|INSTVL|130|CONTINUOUS|ByLineWeightDefault|
|INSUL|white|CONTINUOUS|ByLineWeightDefault|
|LIGHTING|131|CONTINUOUS|ByLineWeightDefault|
|LOCK|60|CONTINUOUS|ByLineWeightDefault|
|LOWVOLT|60|CONTINUOUS|ByLineWeightDefault|
|MANVL|130|CONTINUOUS|ByLineWeightDefault|
|MATCHLINE|11|PHANTOM|ByLineWeightDefault|
|OCS|magenta|CONTINUOUS|ByLineWeightDefault|
|OS|10|CONTINUOUS|ByLineWeightDefault|
|PHONE|131|CONTINUOUS|ByLineWeightDefault|
|PIPELINE|150|CONTINUOUS|ByLineWeightDefault|
|RAIL|blue|CONTINUOUS|ByLineWeightDefault|
|SAND|white|CONTINUOUS|ByLineWeightDefault|
|SC|10|CONTINUOUS|ByLineWeightDefault|
|SECTION|13|CONTINUOUS|ByLineWeightDefault|
|SL|10|CONTINUOUS|ByLineWeightDefault|
|SM|cyan|CONTINUOUS|ByLineWeightDefault|
|SWC|cyan|CONTINUOUS|ByLineWeightDefault|
|SYMBOL|130|CONTINUOUS|ByLineWeightDefault|
|TEXT|yellow|CONTINUOUS|ByLineWeightDefault|
|TTEXT|9|CONTINUOUS|ByLineWeightDefault|
|VIDEO|9|CONTINUOUS|ByLineWeightDefault|
|W|10|CONTINUOUS|ByLineWeightDefault|
|WD|10|CONTINUOUS|ByLineWeightDefault|
|WELLS|green|CONTINUOUS|ByLineWeightDefault|
|WF|11|CONTINUOUS|ByLineWeightDefault|
|WU|cyan|CONTINUOUS|ByLineWeightDefault|

Inserted from UGLAYR.dwg. Plant coordinate system is often used. Any additional layers require prior approval from Client AIM.

### 3.10 Date Convention

The date convention is YYYY-MM-DD.

### 3.11 Units

The unit convention for Project is US Customary units (USC).

### 3.12 AutoCAD Legends & Symbols

Project has legend and symbols reference documents for each asset, and they are expected to be used for those assets. If the project creates a brand-new unit on the Project site, they are to use the Upgrader legends and symbols reference documents. Any project that impacts brownfield assets shall use the legend and symbol reference documents for those assets. These documents can be found in Project's Digital Twin.

**Chemicals:**

|Document|Title|
|---|---|
|01.0000.000.041.01|Project Styrene Project P&ID Legends and Symbols|

**Refinery:**

|Document|Title|
|---|---|
|00_0000_000_041_01|Flow Diagram Symbols for Piping, Valves and Equipment|
|00_0000_000_041_02|P&ID Instrument Identification Letters, Symbols and Loop Numbering|
|00_0000_000_041_03|P&ID Instrument Identification Letters, Symbols & Loop Numbering|
|00_0000_000_041_04|Piping Instrument Diagram All Units Standard Details - Sampling Systems|
|00_0000_000_041_19|P&ID Instrument Identification Letters & Symbols|

**Upgrader:**

|Document|Title|
|---|---|
|200.0000.000.041.018|P&ID All Units Page 1 of 2|
|200.0000.000.041.019|P&ID All Units Page 2 of 2|
|200.0000.000.041.020|P&ID All Units Instr ID Letters and Loop No|
|200.0000.000.041.021|P&ID All Units Function Designations, ID Symbols, Loop ID|
|200.0000.000.041.022|P&ID All Units Instr ID Letters Symbols Loop ID|
|200.0000.000.041.023|P&ID 400 Units Pressure Instrument Connection Details|
|200.0000.000.041.024|P&ID 400 Units Level Instrument Connection Details|
|200.0000.000.041.025|P&ID 400 Units Flow Element Connection Details 1 of 2|
|200.0000.000.041.026|P&ID 400 Units Flow Element Connection Details 2 of 2|
|200.0000.000.041.027|P&ID All Units Flow Diagram Symbols for Equipment Page 1 of 2|
|200.0000.000.041.028|P&ID All Units Flow Diagram Symbols for Equipment Page 2 of 2|
|200.0000.000.041.029|P&ID 200 Units Standard Details - Sampling Systems|
|200.0000.000.041.030|P&ID 400 Units Standard Details - Sampling Systems|

### 3.13 Deliverables

1. Technical drawings shall use black ink only.
2. The final version of a technical drawing shall be delivered in electronic form in both native format and PDF. See Section 9.4 for vendor document standards (they differ).
3. The content of the final drawing transmitted to Client Project shall be identical to the latest check plot and the drawing displayed on the screen when last saved.
4. All drawings transmitted to Client Project shall have their drawing sheet origin set to 0,0 in paper space.

### 3.14 Snap Settings

All drawings to be done with snap settings. All new drawings shall be set up with snap set to 0.5mm.

### 3.15 AutoCAD Pen Plotting Standards

#### 3.15.1 Reserved Pen Numbers, Widths, Colours

To ensure standard and consistent quality for plotted drawings, the following pen numbers, pen widths and assignments must be observed.

The AutoCAD pen width parameter shall also be set to 0.127mm (0.005") at the time of plotting. This pen width setting is critical to the plotting of wide polylines. To ensure plotted line widths match those of the drawing, the correct pen width must be set and the layers containing wide polylines must have a colour assigned pen # 1.

**Table 8.1 - Pen Assignment (Full Scale Plots)**

|Pen #|Pen Width|Colour #|Colour Description|
|---|---|---|---|
|1|0.127mm|7|White|
|2|0.254mm|2|Yellow|
|||3|Green|
|||5|Blue|
|||13|Pastel Red Shade|
|||14|Solid Red Shade|
|||15|Pastel Red Shade|
|||130|Cyan|
|||134|Dark Cyan|
|||221|Maroon|
|3|0.381mm|1|Red|
|||8|Dark Grey|
|||9|Grey|
|||12|Dark Red|
|||60|Yellow/Green|
|||131|Cyan|
|4|0.508mm|4|Cyan|
|||10|Red|
|5|0.635mm|6|Magenta|
|||11|Pink|
|6|0.762mm|-|Colours to be Assigned|
|7|0.889mm|150|Turquoise|
|8|1.016mm|-|Colours to be Assigned|
|9|1.143mm|-|Colours to be Assigned|

**Table 8.2 - Alternate Pen Assignments (Reduced Prints, A3 and below)**

|Pen #|Pen Width|Colour #|Colour Description|
|---|---|---|---|
|1|0.1016mm|7|White|
|2|0.1524mm|2|Yellow|
|||3|Green|
|||5|Blue|
|||13|Pastel Red Shade|
|||14|Solid Red Shade|
|||15|Pastel Red Shade|
|||130|Cyan|
|||134|Dark Cyan|
|||221|Maroon|
|3|0.2540mm|1|Red|
|||8|Dark Grey|
|||9|Grey|
|||12|Dark Red|
|||60|Yellow/Green|
|||131|Cyan|
|4|0.3048mm|4|Cyan|
|||10|Red|
|5|0.5080mm|6|Magenta|
|||11|Pink|
|6|0.600mm|-|Colours to be Assigned|
|7|0.500mm|150|Turquoise|
|8|0.700mm|-|Colours to be Assigned|
|9|0.800mm|-|Colours to be Assigned|

---

## 4. Client Technical Document and Data Storage

Client technical data and documents shall be viewed and maintained in their source application and location using the source file type specified, with native format being the default requirement.

|Document and Data Type|Refinery/File Type|Upgrader Base/File Type|Upgrader Expansion/File Type|Chemicals/File Type|Exception & Notes|
|---|---|---|---|---|---|
|Vendor Documents and Documents|ASSAI SCT_OPS Native or PDF|ASSAI SCT_OPS Native or PDF|ASSAI SCT_OPS Native or PDF|ASSAI SCT_OPS Native or PDF||
|Instrumentation Datasheets|SPI Database|SPI Database|SPI Database|SPI Database|Rupture Disks and RVs, PRVs (see below)|
|Instrumentation Loop and Wiring Diagrams|ASSAI SCT_OPS .dwg/.dgn|ASSAI SCT_OPS and SPI (existing loops/wiring location determines new entry location)|ASSAI SCT_OPS and SPI (existing loops/wiring location determines new entry location)|ASSAI SCT_OPS .dwg/.dgn||
|LDTs|ASSAI SCT_OPS Excel|ASSAI SCT_OPS Excel|SPP&ID Uploaded to ASSAI SCT_OPS PDF|ASSAI SCT_OPS Excel||
|Rupture Disks, RVs and PRVs|ASSAI SCT_OPS PDF/Excel|SPI (Datasheets), ASSAI SCT_OPS (Calculations)|SPI (Datasheets), ASSAI SCT_OPS (Calculations)|ASSAI SCT_OPS PDF/Excel||
|P&IDs|ASSAI SCT_OPS|ASSAI SCT_OPS|SPP&ID, ASSAI SCT_OPS PDF copy|ASSAI SCT_OPS||
|Fieldbus Segment Diagrams|ASSAI SCT_OPS .dwg/.dgn|SPI|SPI|ASSAI SCT_OPS .dwg/.dgn||
|Power Distribution Plot Plans|||||Not being added to the tech library; existing ones will be kept updated|
|3-D Models|No reliable updated model|No reliable updated model (Quest is in S3D)|PDS Isometrics, plans and details; ASSAI SCT_OPS PDF copy|No reliable updated model||
|Non-OEM Repairs and Modifications|||||Before 2018: ASSAI SCT_OPS (hard copy scan); 2018-2022: Machinery SharePoint; 2022-Present: WIMs|
|All other engineering documents|Native format in ASSAI SCT_OPS .dwg/.dgn|Native format in ASSAI SCT_OPS .dwg/.dgn|Native format in ASSAI SCT_OPS .dwg/.dgn|Native format in ASSAI SCT_OPS .dwg/.dgn||

---

## 5. Client Technical Document Revision Procedures

### 5.1 New Client Critical Technical Documents

When issuing a new critical Client technical document for project execution, the following requirements shall be met:

**Drawing Title:** The master drawing title text shall match the details shown in the Contractor's Master Document Register and the SCT.AIM.TMP.1 Projects Documents and Drawings Log.

**Border (Only applicable to Existing Client Technical Drawings):** During a document revision, a temporary border shall be applied outside the existing master border. Client Project does not dictate the look of this external border but requires the border to have:

1. The master revision description and revision block crossed out, with the temporary border having a revision block and description area for project updates.
2. Project number/code.
3. The date and document status code.
4. The title of a drawing shall not be altered except to correct spelling mistakes. If a change is required for reasons other than spelling, the existing drawing number shall be voided and replaced with a new number.

New Client technical documents created within other applications outside of AutoCAD will be issued in PDF format with the master data claimed in the application. SPI standard templates are suitable for documents generated in SPI.

**Revisioning:** See SCT.AIM.PO.4 Revision Policy. Note: documents stored in SPI follow a different revision workflow (see SCT.AIM.ST.10 for Upgrader and SCT.AIM.ST.6 for Refinery & Chemicals).

**Revision Indicators:** The place on the drawing where a revision is made shall be indicated by a triangle containing the appropriate revision code with a cloud surrounding the changes. Exceptions:

1. If the revision constitutes a complete re-draw, a note on the new drawing may be used instead of revision triangles and clouds.
2. For Voids, Retired in Place, Supersede and DWG/CAL revision changes, see Section 6.5.

**Stamps:** Client Project does not provide the stamps that the project is expected to apply. Examples include: Issued for Construction, Issued for Review, For MOC # Use Only, CWP #-[ASSET]-[MOC #].

1. If the document is critical, it shall have a stamp "Client Critical Document As-Built Information Required" and a stamp indicating "Working Copy of Client Critical Document".
2. If the document is non-critical, it shall have a stamp "Working Copy".

**Company Disclaimers:** At the EPC's discretion.

**Standard Issue Codes:** See the Document Status table below. Every issued document shall have one of these codes applied.

**File Compatibility:** All AutoCAD drawings shall be saved in AutoCAD 2010 version compatibility: Save As - "AutoCAD 2010/LT 2010 Drawing (*.dwg)". If created in Microstation, it shall be reviewed in AutoVUE by the engineering designer to assure proper viewing.

**File Name:** The filename shall follow: [CLIENT TECHNICAL DOCUMENT NUMBER]_V[#].[FILETYPE]

**DWG & CAL:** When both a DWG and CAL file are required to produce one image, both documents are expected to be issued together.

**Appendixes:** Where appendices are part of the document, reference Section 2.9 for requirements.

**Document Status:**

|Acronym|Full Text|Examples Of|
|---|---|---|
|ASB|As-Built|Vendor documents|
|CAN|Cancelled|Any document pulled for the project that is no longer needed|
|IFA|Issued for Approval|BDEP, BFD after review and comment incorporation|
|IFB|Issued for Bid|MR|
|IFC|Issued for Construction Approval|Any document requiring construction resource action, including demolition|
|IFD|Issued for Design Approval|BDEP, BFD after approval|
|IDM|Issued for Demolition|Portion of document being removed; SPI datasheets for decommissioning|
|IFE|Issued for Estimate|Procurement|
|IFF|Issued for Fabrication|Modules|
|IFH|Issued for HAZOP|Working P&ID reviewed during HAZOP session|
|IFI|Issued for Information|Sheets/info transmitted outside larger IFR/IFD packages|
|IFP|Issued for Purchase Approval|Instrument Datasheets, Tagged Equipment|
|IFQ|Issued for Quotation|MR|
|IFR|Issued for Review|Any document that gets reviewed|
|IFV|Issued for Void|Physical asset described in the document no longer exists|
|SUP|Superseded|Document replaced by new document with different number|
|RIP|Retired in Place|Physical asset exists but is inactive (air-gapped)|
|IFU|Issued for Use|HAZOP reports, short-circuit study, area classification report|
|RLM|Redline Markup|Documents required to be as-built but currently provided as redline markup|

**Cancellation:** If a new critical Client technical document is to be cancelled at any time during the project, the project is responsible for notifying Client by returning the SCT.AIM.F.1 routing form with the "Cancellation of Placeholder" tab filled out. The Client Technical Document Number will be de-activated and not deleted.

**'New' Critical Document 'Excerpts':** There are documents that appear non-critical because they are brand new documents that are excerpts from existing Client critical documents and do not use the existing critical document number (e.g. electrical schedules, LDTs, SFDs, PFDs). During the project, these are assigned a number per PG-009. Their content shall be merged to the existing critical master document at closeout, so they shall be clearly stamped: "The information contained on this document shall be transferred to master [#] during as-building."

#### 5.1.1 New Client Non-Critical Technical Documents

There are 2 types of non-critical documents with defined paths at closeout:

1. Issuing new non-critical documents for project execution will in some cases be subject to the same requirements as critical documents in terms of border, revision control, file format, etc. Types may include structural drawings, calculations, Installation and Operation Manuals (see Section 2.4 eMOC Checklist for qualifying types). If the non-critical document fits this criterion, issue it following Section 5.1 standards.
    
    - Note 1: This does not include bill of materials, photographs, extra vendor drawings or construction detail drawings.
    - Note 2: The primary difference between these and critical documents is that these will not be as-built. Instead, the IFC revision will be uploaded to the technical library upon close out. See SCT.AIM.PR.1 for execution details.
2. There are non-critical documents not retained at the conclusion of the project life cycle; these will be marked as sketches (see Section 3.4.2.1).
    

---

## 6. Existing Client Technical Document Revision Procedures

### 6.1 Retrieving Existing Client Technical Documents

When a document currently residing in the technical library is revised by a project, it shall be retrieved by the EPC/PEC through gaining access to the proper systems.

1. Access for those with an external email: Contact your Third-Party Access representative or SCT-REF-TPA-REQUESTS@shell.com.
2. Access for those with a Client email: Visit the respective SharePoint pages for SmartPlant Instrumentation, Digital Twin, and AVEVA Work Task.

Some documents/content in the Digital Twin are 'copies' of master data from SPI, SPP&ID and S3D that require project change directly in those tools. See Section 1.5 Related Documents for standards and procedures.

The AIM department is not involved in day-to-day retrieval of technical documents for project use. Due to site age, some documents require a DWG and a CAL file to produce one image; ensure both are retrieved if applicable. Also, some documents may have embedded appendixes; ensure all appendices are retrieved.

### 6.2 Identifying Existing Client Technical Documents Under Multiple Project Change

Client Project does not track when a document has been retrieved for a project until IFR has been issued for the Projects department and IFC has been issued for the EDR process.

### 6.3 Issuing Existing Client Critical Technical Documents

See Section 5.1 for requirements. See Section 1.5 for standards and procedures related to SPI, SPP&ID or S3D.

When revising an existing critical document where a demolition revision shall be issued:

1. The demolition document shall be a new revision of the existing document.
2. The demolition document shall be issued for construction.
3. The demolition document shall not be as-built.
4. The demolition document can be identified by adding the letter "D" to the end of the existing document number (e.g. 24_1513_000_063_23D).

### 6.4 Issuing Existing Client Non-Critical Documents

See Section 5.1.1 bullet 1 for applicable types and direction.

When revising an existing non-critical document where a demolition revision shall be issued:

1. The demolition document shall be a new revision of the existing document.
2. The demolition document shall be issued for construction.
3. The demolition document shall not be as-built.
4. The demolition document can be identified by adding the letter "D" to the end of the existing document number (e.g. 24_1513_000_063_23D).

### 6.5 Deleted, Superseded, Retired in Place and DWG/CAL Overlay Removal

#### 6.5.1 Deleted Documents (Issued for Void)

Documents that must be deleted or cancelled during project work (e.g. equipment removed and not replaced) must remain in ASSAI but will be marked inactive and not visible through a standard search. Requirements:

1. A diagonal cross shall be drawn through the document with "Issued for Void" watermarked across all pages.
2. A new hard revision shall be applied with the description "Issued for Void per MOC [#]".
3. Adjust the filename to: "(ISSUED FOR VOID) [CLIENT DOCUMENT NUMBER]_V[#].dwg"
4. If the document does not have a version number, use: "(ISSUED FOR VOID) [CLIENT DOCUMENT NUMBER]_VNA.dwg"

#### 6.5.2 Superseded Documents

A document is superseded when its information has been moved to another document or the document number has changed. The original must be maintained within ASSAI, will remain active, and shall refer to the new drawing. Requirements:

1. A diagonal cross shall be drawn with "Superseded by: New Document No. [#]" watermarked across all pages.
2. A new hard revision with description "Superseded by: New Document [#] Per MOC [#]".
3. Adjust the filename to: "(SUPERSEDED BY #) [CLIENT DOCUMENT NUMBER]_V[#].dwg"
4. If no version number exists, use: "(SUPERSEDED BY #) [CLIENT DOCUMENT NUMBER]_VNA.dwg"

#### 6.5.3 Retired in Place Documents

A document may represent an asset that has been abandoned or retired in place. These must be maintained within ASSAI but will be marked inactive and not visible through standard search. Requirements:

1. A diagonal cross with "Retired in Place" watermarked across all pages.
2. A new hard revision with description "Retired in Place Per MOC [#]".
3. Adjust the filename to: "(RETIRED IN PLACE) [CLIENT DOCUMENT NUMBER]_V[#].dwg"
4. If no version number exists, use: "(RETIRED IN PLACE) [TECHNICAL DOCUMENT NUMBER]_VNA.dwg"

#### 6.5.4 DWG and CAL Overlay Converted to One DWG Document (Issued for Void)

Due to the length of time some Client Project assets have been in place, there are original hard copy documents that have been rasterized to .cal file format as a base for AutoCAD as-building changes. When the .cal file is no longer needed to support the .dwg file:

1. Indicate on the .dwg revision block descriptor: "CAL File No Longer Required, As-Built Per MOC [#]".
2. Adjust the filename of the .cal file to: "(ISSUED FOR VOID) [CLIENT DOCUMENT NUMBER]_V[#].cal"

---

## 7. As-Building

As-building at Project is targeted to be completed within 180 days from turnover of project to operations. This target follows the Client DEP 82.00.10.30-Gen Engineering Information Specification, Section 2.3 Delivery Timing Requirements: "all engineering information identified as part of the project scope, shall be delivered within six months after start-up." To help deliver this, all as-building shall be triggered 2 weeks after the ready-for-start-up date as determined by the project schedule.

### 7.1 As-Building New Client Critical Documents

A new Client critical document is considered the Client "Master" file. As-building shall be completed as follows:

**Redline Generation & Triggering As-Building:**

1. Field construction redline changes are incorporated into the latest engineered IFC document and triggered by the field contractor (see SCT.AIM.PR.1 Section 3.1).
2. Commissioning contractor redlines are issued after field installation redlines and trigger as-building (see SCT.AIM.PR.1 Section 3.2).
3. Fabrication shop redlines are triggered by the Client Project Engineer (see SCT.AIM.PR.1 Section 3.3). These often impact the same documents as construction redlines; all shall be incorporated. If discrepancies exist between fabrication and construction redlines, the construction redline content is assumed correct.
4. Document Impact Assessment Package/Process Document redlines can be developed and triggered by the Client Project Engineer (see SCT.AIM.PR.1 Sections 3.4 and 5.3).

**Redline mark-ups shall follow this standard colour-coding:**

1. Red = Additions
2. Green = Deletions
3. Blue = Information

**Additional requirements:**

1. In some instances, the master data/file exists in SPI, SPP&ID or S3D; all redline mark-ups shall be incorporated into those tools. New technical critical document as-building requirements for SPI are outlined in SCT.AIM.PR.16.
2. If the new Client critical document is only available in native PDF format, it shall be converted to a .CAL file and as-built changes performed as an overlay .DWG. This does not apply to PDFs generated because the master data exists in SPI, SPP&ID, or S3D; in those cases, the PDF is used as a reference and data is updated within the tool itself.
3. If the document has embedded appendices, ensure changed appendices are updated and all appendices are provided as part of master upload.
4. All AutoCAD drawings shall be saved in AutoCAD 2010 version compatibility.
5. All clouds and revision triangles are removed (since the document was created new for this project).
6. Construction notes belonging to this MOC only shall be removed.
7. The project number cell shall be empty.
8. The next hard revision (e.g. 0, 1, 2) shall be applied, including documents marked "As-Built No Change". The MOC # shall be referenced in the revision description block with drafter's and checker's initials and date: "As-Built Per MOC #". All project-related soft revisions shall be removed.
9. For P&IDs, a change list shall be populated (see Section 7.3), except for Vendor P&IDs (see Section 7.3.1).
10. Filename standard: [TECHNICAL DOCUMENT NUMBER]_V[#].dwg (.dgn). For multiple sheets: [TECHNICAL DOCUMENT NUMBER]_Sheet [# of #]_V[#].dwg. Note: Refinery documents use underscores as separators (e.g. 24_0000_000_041_1_V5.dwg).
11. Client project group or project-specific stamps shall be removed. The following electronic stamp shall be added or remain on all new Client critical documents (exempt from SPI): "CLIENT CRITICAL DOCUMENT - AS-BUILT INFORMATION REQUIRED"
12. The as-build team shall determine whether there are additional changes due to any redlines provided. Atypical changes require consultation with the Client Project Engineer.
13. The final version shall be uploaded to its master application in both native format and PDF if accepted.

### 7.2 As-Building Existing Client Critical Documents

When updating an existing Client critical document, the project as-built information is transferred to the Client "Master" file document. Bullets 1-5 from Section 7.1 apply. Differences:

1. Remove the temporary construction border.
2. Remove any Client Project group or project-specific stamps. Ensure the critical stamp from Section 7.1 is on the document. Remove any additional stamps beyond those mentioned.
3. Construction notes belonging to this MOC only shall be removed.
4. The next hard revision shall be added to the master file document revision block, including "As-Built No Change" documents. Reference the MOC # with drafter's and checker's initials and date: "As-Built Per MOC #". Remove all project-related soft revisions.
5. The as-build team shall determine whether additional changes are needed from redlines. Atypical changes require consulting the Client Project Engineer.
6. Filename standard: [TECHNICAL DOCUMENT NUMBER]_V[#].dwg (dgn), [TECHNICAL DOCUMENT NUMBER]_V#.cal, or for multiple sheets: [TECHNICAL DOCUMENT NUMBER]_Sheet [# of #]_V[#].dwg. Note: Refinery documents use underscores as separators.

Existing Client critical document as-building requirements for SPI are outlined in the SPI standards (SCT.AIM.ST.6 for Refinery & Chemicals, SCT.AIM.ST.10 for Upgrader).

**Note:** If an existing critical document has been loaded into ASSAI SCT_OPS but not been as-built (and should have been), it shall follow Section 7.2 guidelines and not be considered a new document.

### 7.3 P&ID As-Building (Not Including Vendor P&IDs)

When updating a P&ID with as-built information, follow Sections 7.1 and 7.2 with these exceptions:

**P&ID Drawing:**

1. The next hard revision shall be added to the master revision block with description "See Change List".
2. Place an X through all revisions in the revision block except the current one on the P&ID. This shall not happen on the P&ID Change List.
3. All clouds and revision triangles shall be removed.
4. Remove the temporary construction border if applied.
5. For Smart Plant P&ID master list, refer to SCT.AIM.IDX.7 - SPPID Drawings List.

**P&ID Change List:**

1. Update with the next hard revision; reference MOC No# with drafter's and checker's initials and date: "As-Built Per MOC [#]". The description shall be completed so a viewer understands exactly what has been changed.
2. All clouds and revision triangles shall be removed.

**Filenames:**

1. P&ID: [TECHNICAL DOCUMENT NUMBER]_V[#].dwg
2. P&ID Change List: [TECHNICAL DOCUMENT NUMBER]R_V[#].dwg

#### 7.3.1 Vendor P&ID As-Building

Skid units or major equipment supplied by vendors may come with their own P&ID on the vendor's letterhead with border.

When newly installed and project closed out, the vendor P&ID turnover shall follow the vendor document upload process (see Section 9.0).

When future changes merit a P&ID revision, the EPC follows issuance standards in Section 6.0. For as-building:

1. The existing vendor P&ID revision block will remain with a strikethrough.
2. The temporary border applied by the EPC will be replaced by a new Client border (from the AIM Forms SharePoint under Drafting & Design - Templates).
3. Revision block and remaining as-built requirements per Section 7.2 will be implemented.
4. A P&ID change list is not created for vendor P&IDs.

---

## 8. Updating Non-Critical Documents

For non-critical documents from a project that need to be updated in their construction state to the technical library, or are being deleted/superseded, the following applies before uploading into ASSAI SCT_OPS:

1. For Issued for Void/Supersede/Retired in Place documents, follow Section 6.5 requirements.
2. If the document has a hard revision higher than the existing document in ASSAI SCT_OPS, upload directly.
3. Previous construction revisions shall remain on the document.
4. If the document has a soft revision, the next hard revision shall be applied.
5. If the document is new to ASSAI SCT_OPS, the first hard revision shall be 0 regardless of project revision.
6. The revision block shall indicate "Issued for Construction MOC [#]" (not applicable for Issued for Void/Supersede/Retired in Place documents).

---

## 9. Vendor Documents

### 9.1 Creating New Vendor Documents

Client Project is not involved in the creation of new vendor documents. Client Project has a collection of templates that may be useful as a reference to vendors on expectations (AIM Forms SharePoint - Drafting & Design - Templates - SCT.AIM.TMP.4).

### 9.2 Review Vendor Documents

Vendor document review is not a process controlled through Client AIM, and thus standards are not set.

### 9.3 Vendor Document Processes

#### 9.3.1 Projects Vendor Document Process

Since August 2022, EPC firms have uploaded new vendor documentation related to projects through ASSAI SCT_MOD, from which it is uploaded to ASSAI SCT_OPS. Some existing vendor documentation is naturally updated as part of a construction work package or change order. To address the gap in remaining existing vendor documentation, Project introduced a Document Impact Assessment Package for all projects not past DG4 before September 1, 2023, ensuring all existing vendor documentation in the technical library is appropriately actioned by the EPC.

For any project that has passed DG4 as of September 1, 2023, it is at the Client Project Engineer's discretion. Options:

1. The Client Project Engineer executes the new vendor document upload and existing document review (see SCT.AIM.PR.1 Section 5.5).
2. The EPC firm executes both (see SCT.AIM.PR.1 Sections 5.5.1 and 5.5.2).
3. The EPC firm executes new vendor document upload (SCT.AIM.PR.1 Section 5.5.1) while the Client Project Engineer actions the existing vendor document review (SCT.AIM.PR.1 Section 5.5.2).

#### 9.3.2 Vendor Document Process - Excluding Projects

The PEC shall follow SCT.AIM.PR.1 Section 6.3 while reviewing this section's content to ensure vendor documents meet these standards.

### 9.4 Vendor Document Standards

1. Only the latest revision of a vendor document shall be submitted for uploading to ASSAI SCT_OPS.
2. All vendor documents shall be turned over in an as-built state.
3. All documents shall be in the format per the purchase order requirements. When no such guidance exists, they shall be submitted in PDF format. All files shall be submitted electronically without security settings applied (e.g. PDF/A).
4. All AutoCAD drawings shall be saved in AutoCAD 2010 version compatibility.
5. Vendor documents (IOM, MRB and individual critical technical documents) shall have a text box applied with: the technical document number provided, revision description (Standard: "Vendor Turnover"), and the revision set to 0 if brand new or the next hard revision if existing. The "CLIENT CRITICAL DOCUMENT - AS-BUILT INFORMATION REQUIRED" stamp shall also be applied only to critical vendor documents.
6. MRB for twinned/tripled/quadrupled equipment: one document shall represent all identical assets. Example: V-2302A and V-2302B MRB will be one document numbered 23_08V-_02-_025.
7. Equipment datasheets for twinned equipment: one datasheet shall represent all identical assets. Example: P-2301A and P-2301B will be one datasheet numbered 23_11P-_01-_035.
8. If the document pertains to more than one asset of different tag sequences or equipment types, 000 shall be used with a more generalized subclass code.
9. Installation and Operating Manuals shall be assigned the "025" document type.
10. Manufacturing Record Books shall be assigned the "021" document type.

### 9.5 New Vendor Manufacturing Record Book Standard

Requirements for MRBs submitted to Client:

1. All MRB turnover documents shall be assigned document type 021.
2. Most MRBs are associated to one piece of equipment; the technical document number shall be assigned accordingly (e.g. 22_08V-_04-_021_01). If the MRB has multiple tags of different equipment, use: 22_0000_000_021_S.
3. ASSAI metadata title standard: MOC [#] [PO #] [Name of Vendor] Title of Document - Equipment Tags.
4. Volumes: the technical document number shall include the volume (e.g. 22_08V-_04-_021_1 VOL 1 of 5, 22_08V-_04-_021_1 VOL 2 OF 5).
5. The vendor shall turn over a complete MRB package to the EPC.
6. The EPC shall extract critical technical documents from the MRB (see SUG.CON.MOC.F.002 for guidance) and assign technical document numbers. Even though extracted into individual files, they shall remain embedded within the MRB but indicate the new technical document number for reference. Future changes to those documents shall be on the stand-alone copies only; the original MRB is not updated.
7. The technical document number shall be applied to the front page of the document (see Section 9.4 bullet 5).
8. An index shall be part of the MRB and bookmarked with related pages.
9. Test reports including hydrotesting, NDE, WPS, API, hardness test, etc. should be included in the MRB, not as separate documents.

---

**Appendix A: MTO Reference Document**

(Refer to original document for appendix content.)