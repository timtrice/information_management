# Document Handling Process
**Current State Overview for Line Managers**

---

## Document Sources
- **Client EDMS** (Outbound folder)
- **Client EDMS** ("Bootleg" folder)
- **Email** (Client/Client's client)

---

## Document Processing Pathways

### 🟢 CONTROLLED DOCUMENTS
**Source:** Client EDMS with transmittal form  
**Processing:** Assigned transmittal number  
**Storage:** Company EDMS "Documents" folder + Network Drive "17-Deliverables"  
**Status:** "Sole source of truth"  
**Metadata:** Captured from transmittal form  
**Revision History:** ✅ Maintained

### 🔴 UNCONTROLLED DOCUMENTS
**Source:** Client EDMS "Bootleg" folder OR Email  
**Processing:** Assigned EML document number (AAA-BBB-CCC-0000)  
**Storage:** Network Drive "6-Correspondence"  
**Status:** Correspondence only  
**Metadata:** ❌ Not captured electronically  
**Revision History:** ❌ Not maintained

---

## Final Storage

**Controlled:**
- Company EDMS
- Network Drive (17-Deliverables)

**Uncontrolled:**
- Network Drive (6-Correspondence)

---

## Legend

🟢 **Controlled Documents** - Proper transmittal process  
🔴 **Uncontrolled Documents** - Email/Bootleg folder

---

## ⚠️ Current Issues & Risk Factors

### Mixed Document Status
Same document may exist as both Controlled and Uncontrolled, potentially with different revisions

### No Metadata Definitions
Codes like "A1", "B1", "B2" used but meanings unknown (Client denied information management documentation)

### No POR Mapping
Cannot map Professional of Record to discipline/document type combinations

### Version Control Gaps
Uncontrolled documents may have later revisions than Controlled documents - no tracking system in place

### Quality Control Breakdown
Email submissions bypass industry-standard ISO procedures

### Client Instruction Override
Despite raised concerns, Client instructed to continue current process

---

## 👤 POR Responsibility

**Professional of Record (POR)** must validate Uncontrolled documents against Controlled documents. Any discrepancies should be raised with Client. However, DC lacks proper mapping tools to streamline this process.

---

## Key Definitions

- **EDMS:** Electronic Document Management System
- **DC:** Document Control
- **POR:** Professional of Record
- **EML Format:** AAA-BBB-CCC-0000 (Project-Client-FileType-Sequential)