# 📘 Meeting Notes Generator (Senior PM Standard)

## Overview
This prompt is designed to generate **structured, executive-quality meeting notes** from a project status meeting transcript.

It applies **Senior Project Manager governance standards** to extract:

- Decisions  
- Actions  
- Issues  
- Risks  
- Work package updates  
- Key discussion context  

The output is optimised for **formal project records, RAID logs, and executive reporting**.

---

## 🎯 Key Outcomes

Using this prompt ensures:

- Clear separation of **decisions vs discussions**
- Full traceability to the **source transcript**
- Structured outputs suitable for **Word, Excel, or SharePoint**
- Immediate usability for **project governance and delivery tracking**
- Consistent application of **RAID discipline**

---

## 👥 Target Audience

- Project Managers  
- Delivery teams  
- Project governance forums (SteerCo, PMO)  

---

## 🇦🇺 Language Standard (Mandatory)

All outputs:

- Use **Australian English**  
- Follow professional, formal workplace tone  
- Avoid casual, speculative, or subjective language  

---

## 🧠 What the Prompt Does

The prompt:

1. Analyses a full meeting transcript  
2. Identifies the meeting date  
3. Extracts key delivery information  
4. Structures outputs into governance-ready formats  
5. Applies strict rules to avoid inference or ambiguity  

---

## 📦 Output Structure

The generated output includes:

### 1. Overall Status Summary
- Current project phase/status  
- Key progress  
- Constraints, risks, and dependencies  
- Milestones or phase transitions  

### 2. Work Package Updates
Structured table of:

- Progress since last update  
- Key milestones  
- Issues/blockers  
- Next focus  

---

### 3. Decisions Register

| Field | Description |
|------|-------------|
| Decision ID | Unique identifier (DMM.DD.NN) |
| Decision | Confirmed outcome |
| Owner | Accountable party (if stated) |
| Context | Supporting rationale |

---

### 4. Actions Register

| Field | Description |
|------|-------------|
| Action ID | Unique identifier (AMM.DD.NN) |
| Action | Specific task |
| Owner | Responsible person |
| Due Date | If stated |
| Status | Optional |

---

### 5. Issues Register

| Field | Description |
|------|-------------|
| Issue ID | Unique identifier (IMM.DD.NN) |
| Issue | Current problem |
| Impact | Delivery impact |
| Owner | If stated |
| Status | If stated |

---

### 6. Risks Register

| Field | Description |
|------|-------------|
| Risk ID | Unique identifier (RMM.DD.NN) |
| Risk | Future uncertainty |
| Potential Impact | Delivery implication |
| Likelihood | If stated |
| Owner | If stated |
| Mitigation | If stated |

---

### 7. Key Discussion Points
- 3–5 concise bullets  
- Only critical context supporting outcomes  

---

## 🔢 ID Convention

All artefacts follow strict ID formatting:

| Type      | Format      | Example     |
|----------|------------|------------|
| Action   | AMM.DD.NN  | A05.10.01  |
| Decision | DMM.DD.NN  | D05.10.01  |
| Issue    | IMM.DD.NN  | I05.10.01  |
| Risk     | RMM.DD.NN  | R05.10.01  |

**Rules:**
- Reset numbering per category  
- Sequence based on transcript order  
- Do not skip or reuse IDs  

---

## ⚖️ Governance Rules (Critical)

- No inference of:
  - Owners  
  - Dates  
  - Decisions  
  - Risk ratings  

- Decisions must be:
  - Explicitly agreed  
  - Written as completed outcomes  

- Actions must be:
  - Specific and executable  

- Risks and Issues must:
  - Be clearly distinguishable  
  - Not be misclassified  

- All outputs must be:
  - **Traceable to the transcript**
  - **Standalone and audit-ready**

---

## ✅ Quality Checks

Before finalising output, ensure:

- Decisions, Actions, Risks, Issues are distinct  
- ID conventions are correct and sequential  
- No assumptions or inferred data  
- Output is concise and structured  
- Language complies with Australian standards  

---

## 🚀 How to Use

1. Copy the prompt into **Copilot / GPT / Agent Builder**  
2. Provide a **meeting transcript**  
3. Run the prompt  
4. Copy output into:
   - Meeting minutes  
   - RAID log  
   - Status reports  

---

## 📁 Suggested Repository Structure

