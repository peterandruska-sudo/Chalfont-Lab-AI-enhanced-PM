📘 README – Meeting Notes Prompt (Project-Focused)
✅ Overview
This prompt is designed to generate structured, action-oriented meeting notes from project status update transcripts.
It is optimised for:

Project Managers
Meeting participants
Governance-aligned project environments (e.g. RAID-driven delivery)

The output is clear, structured, and immediately usable, with a strong emphasis on:

Decisions
Actions
Work package progress
Traceability to source discussions


🎯 Use Case
Use this prompt when you need to:

Convert meeting transcripts into clean, structured notes
Capture decisions and actions in a consistent format
Provide a single source of truth for meeting outcomes
Enable rapid follow-up without re-reading transcripts

Typical inputs:

Teams meeting transcript
Workshop transcript
Project status meeting notes (raw)


📥 Input Requirements
The prompt expects:

A complete meeting transcript
Ideally includes:

Meeting date (used for ID generation)
Named speakers
Clear discussion flow




📤 Output Structure
The prompt generates five structured sections:
1. Overall Status Summary

Current project position
Key progress
Constraints, risks, dependencies
Phase transitions or milestones

2. Work Package Updates
| Work Package | Progress | Milestones | Issues / Blockers | Next Focus |

Only includes work packages explicitly discussed
Structured for quick scanning

3. Decisions Register
| Decision ID | Decision | Owner / Accountable | Context / Rationale |

Captures confirmed decisions only
No proposals or discussions

4. Actions Register
| Action ID | Action Description | Owner | Due Date | Status |

Captures all follow-up activities
Focus on accountability and execution

5. Key Discussion Points (Optional)

Supporting context only
Limited to critical insights


🆔 ID Convention (Critical)
All Decisions and Actions follow a structured ID format:

Actions: A<MM>.<DD>.<NN>
Decisions: D<MM>.<DD>.<NN>

Example:

A05.10.01 → First action from 10 May
D05.10.01 → First decision from 10 May

Rules:

MM = Month (2 digits)
DD = Day (2 digits)
NN = Sequential number starting from 01
Separate numbering for Actions and Decisions
IDs must follow order of appearance in the transcript
No gaps or duplication


⚙️ How to Use
Step 1 – Copy the Prompt
Copy the full prompt into your tool (e.g. Copilot, ChatGPT, Agent Builder).
Step 2 – Attach Transcript
Paste or upload the meeting transcript.
Step 3 – Run the Prompt
Execute the prompt to generate the structured output.
Step 4 – Review Output
Quickly check:

Decisions vs Actions separation
ID format compliance
Completeness of work package updates


✅ Quality Controls (Built In)
The prompt enforces:

✅ Australian English (spelling + tone)
✅ No inferred content
✅ Strict decision/action classification
✅ Traceability to transcript
✅ Structured, non-narrative output
✅ Practical, execution-ready notes


⚠️ Known Limitations


If the meeting date is missing, IDs may default incorrectly
→ Recommend including date in transcript or metadata


If ownership is not stated, fields remain blank
→ This is intentional (no inference allowed)


Highly unstructured transcripts may reduce output quality
→ Best results with speaker-labelled transcripts



💡 Best Practices
To maximise output quality:

✅ Ensure transcript includes speaker identifiers
✅ Include clear meeting date
✅ Run prompt immediately after meetings (fresh context)
✅ Pair with RAID log updates for governance tracking
✅ Store outputs in SharePoint or project artefacts repository


🔁 Reuse & Integration
This prompt works well with:

Microsoft 365 Copilot (Word / Teams / Loop)
Copilot Agent Builder (as a system instruction)
GitHub repositories for prompt libraries
Project governance workflows (RAID logs, status reports)


🚀 Optional Enhancements
Consider extending with:

RAID log auto-generation
Risk scoring (Likelihood × Consequence)
Automated executive summary extraction
Integration into project reporting templates


📌 Summary
This prompt provides a repeatable, governance-aligned way to turn meeting transcripts into:

Clear decisions
Actionable next steps
Structured project insights

Designed for real-world project delivery, not just summarisation.
