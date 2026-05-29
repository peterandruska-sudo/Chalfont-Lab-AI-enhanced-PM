# Purpose
Review a project status update meeting transcript and generate clear, structured meeting notes for the Project Manager and meeting participants.

# Audience Context
- Primary audience: Project Manager and meeting participants
- The output must:
  - Enable rapid understanding of key outcomes
  - Clearly distinguish decisions from discussions
  - Provide actionable next steps with ownership

# Language Requirement (Mandatory)
- All output must be written in **Australian English**
- Use Australian spelling conventions (e.g. "organisation", "programme", "favour", "authorise")
- Maintain a professional, neutral, and formal tone suitable for workplace documentation in Australia

# General Guidelines
- Be concise, direct, and outcome-focused
- Prioritise clarity over completeness
- Use project terminology, deliverable names, and work package structure exactly as stated
- DO NOT infer, reinterpret, or introduce information not explicitly stated
- Avoid narrative summaries — use structured bullets and tables
- Focus on decisions, risks, dependencies, and delivery impact

# Extraction Rules (Critical)
- A **Decision** = a confirmed outcome, agreement, or direction
- An **Action** = a specific task that requires follow-up work
- Do NOT convert discussions, intentions, or opinions into decisions/actions
- If ownership or dates are not stated, leave fields blank (do not infer)
- Ensure all items can be directly traced to the transcript

# ID Convention (Mandatory)
All Decisions and Actions must follow this ID format:

- **Actions:** A<MM>.<DD>.<NN>
- **Decisions:** D<MM>.<DD>.<NN>

Where:
- MM = month of the meeting (2 digits)
- DD = day of the meeting (2 digits)
- NN = sequential number starting at 01

Example:
- A05.10.01 = First action identified from a meeting held on 10 May
- D05.10.01 = First decision identified from the same meeting

Rules:
- Reset NN numbering separately for Actions and Decisions
- Number sequentially in order of appearance in the transcript
- Do not skip or reuse numbers

# Instructions
1. Identify the meeting date from the transcript (or metadata if provided)
2. Analyse the full meeting transcript
3. Extract and organise key information into the sections below

# Output Structure

## 1. Overall Status Summary
Provide a concise, factual summary:
- Current project position (e.g. Discovery complete, Build phase upcoming)
- Key progress achieved
- Key constraints, risks, or dependencies raised
- Any confirmed phase transitions or delivery milestones

## 2. Work Package Updates
Only include work packages explicitly referenced

| Work Package | Progress Since Last Update | Key Milestones | Issues / Blockers | Next Focus |
|--------------|--------------------------|----------------|-------------------|------------|

- Use short, factual statements (no narrative)
- Do not create work packages if not clearly stated

## 3. Decisions Register
Capture confirmed decisions only

| Decision ID | Decision | Owner / Accountable | Context / Rationale |
|-------------|----------|---------------------|---------------------|
| DMM.DD.01   |          |                     |                     |

- Use the ID convention defined above
- Decisions must be:
  - Explicitly stated or clearly agreed in the meeting
  - Written as completed outcomes (not proposals)
- Exclude suggestions, risks, or contingencies

## 4. Actions Register
Capture all follow-up actions

| Action ID | Action Description | Owner | Due Date | Status |
|-----------|--------------------|-------|----------|--------|
| AMM.DD.01 |                    |       |          |        |

- Use the ID convention defined above
- Actions must be:
  - Specific and executable
  - Clearly attributable to an owner (if stated)
- Include implicit follow-ups only if clearly implied by commitment language (e.g. “I’ll”, “We need to”)

## 5. Key Discussion Points (Minimal)
- Capture only critical context that:
  - Explains decisions or risks
  - Provides important background for participants
- Limit to 3–5 concise bullet points

# Quality Checks (Mandatory)
- Decisions and Actions are distinct (no overlap)
- All IDs follow the correct format and sequencing
- No inferred ownership, dates, or outcomes
- All content is traceable to the transcript
- Output is readable standalone (no transcript required)
- Language complies with Australian English conventions
- Prioritise clarity, usability, and immediate actionability
