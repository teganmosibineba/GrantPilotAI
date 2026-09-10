# GrantPilot AI

> An autonomous opportunity discovery and application-readiness agent for African students, researchers, and early-career professionals.

## Overview

GrantPilot AI helps students and researchers identify, evaluate, prioritise, and prepare for scholarships, fellowships, research grants, and funded academic opportunities.

Finding suitable academic opportunities is often a repetitive and time-consuming process. Applicants must search multiple platforms, interpret eligibility requirements, confirm funding conditions, track deadlines, prepare similar documents, and decide which opportunities deserve immediate attention.

GrantPilot AI reduces this workload by using the Strands Agents SDK and Amazon Bedrock to analyse opportunities, compare them with an applicant's profile, explain compatibility, generate application checklists, and prepare editable document drafts.

The system automates low-risk planning activities while keeping consequential external actions, such as sending messages or submitting applications, under human control.

## Hackathon Track

**Professional Agents**

GrantPilot AI supports students, researchers, and professionals by reducing repetitive and judgment-heavy work involved in finding and preparing applications for academic opportunities.

## The Problem

Many qualified students and researchers, particularly those in Africa, miss valuable academic opportunities because:

- Opportunity information is distributed across many websites and platforms.
- Eligibility requirements are often long or difficult to interpret.
- Funding information may not be immediately clear.
- Applicants repeatedly prepare the same types of documents.
- Multiple deadlines are difficult to monitor.
- Applicants may spend time on opportunities for which they are not eligible.
- Existing search platforms frequently provide results without personalised explanations.
- Applicants may not know which opportunity should receive the highest priority.

These difficulties create an information and administrative burden that can prevent capable candidates from completing strong applications on time.

## The Solution

GrantPilot AI provides a structured, explainable, and safety-conscious workflow.

The application allows a user to:

1. Create an academic and professional profile.
2. Add genuine scholarships, PhD positions, fellowships, or research grants.
3. Compare each opportunity with the saved profile.
4. Calculate an explainable compatibility score.
5. identify funding, eligibility, and deadline concerns.
6. Rank opportunities by priority.
7. Generate an application checklist.
8. Produce an editable application draft.
9. Record human review before any consequential action.
10. Maintain an audit trail of the agent's activities.

GrantPilot AI does not automatically submit applications, upload personal documents, or contact third parties. These actions remain under the applicant's control.

## Target Users

GrantPilot AI is designed for:

- Undergraduate and postgraduate students
- Prospective PhD candidates
- Academic researchers
- Early-career professionals
- Scholarship applicants
- Fellowship applicants
- Research-grant applicants
- Career advisers and academic mentors

The initial focus is on applicants in Africa, but the workflow can support users in other regions.

## Why It Matters

Access to academic funding can influence a person's education, research career, economic opportunities, and capacity to contribute to society.

Many applicants do not lack ability. Instead, they lack the time, tools, and structured support required to find and prepare for suitable opportunities.

GrantPilot AI helps applicants make better decisions by:

- Reducing repetitive administrative work
- Making eligibility analysis easier to understand
- Prioritising fully funded opportunities
- Providing transparent reasons for recommendations
- Highlighting missing or unverified information
- Producing actionable preparation checklists
- Keeping the applicant in control of important decisions

## Key Features

### Applicant Profile

The user can save:

- Name
- Email address
- Country
- Highest qualification
- Academic field
- Technical and professional skills
- Research interests
- Funding requirements

The profile becomes the foundation for opportunity analysis.

### Opportunity Collection

Users can add opportunities using information from official announcements.

The application records:

- Opportunity title
- Organisation
- Research field
- Application deadline
- Funding status
- Official URL
- Eligibility requirements
- Description
- Required documents

### Explainable Compatibility Scoring

GrantPilot AI calculates a compatibility score using:

- Alignment with the applicant's field
- Skill and research-interest overlap
- Funding availability
- Geographic eligibility
- International-applicant eligibility
- Deadline status and urgency

Every result includes supporting reasons and concerns requiring verification.

### Strands Agent Analysis

The Strands agent can use custom tools to:

- Inspect the applicant profile
- List saved opportunities
- Evaluate a selected opportunity
- Create an application-readiness plan

The agent receives structured information from these tools and produces a clear recommendation and action plan.

### Opportunity Prioritisation

Each analysed opportunity is assigned a priority:

- **High Priority**
- **Medium Priority**
- **Low Priority**

This helps applicants concentrate on opportunities with stronger compatibility and manageable deadlines.

### Application Checklist

GrantPilot AI creates a checklist that may include:

- Verifying official eligibility
- Updating the curriculum vitae
- Preparing transcripts
- Drafting a statement of purpose
- Preparing a research proposal
- Requesting recommendation letters
- Confirming English-language requirements
- Preparing passport documents
- Reviewing the final application

The checklist changes when specific document requirements are detected.

### Drafting Assistant

The application can prepare editable drafts for:

- Statement-of-purpose outlines
- Application emails
- Research-interest summaries

Users must review all generated content and confirm that every factual claim is correct before using it.

### Human Approval Gate

GrantPilot AI separates actions according to their level of risk.

Low-risk actions can be performed automatically:

- Analysing opportunities
- Calculating compatibility
- Ranking opportunities
- Creating checklists
- Preparing editable drafts

High-risk actions require explicit human approval:

- Sending an email
- Uploading a personal document
- Contacting an institution
- Submitting an application
- Making a financial commitment

The current prototype does not perform high-risk external actions.

### Audit Trail

The system records important activities, including:

- Profile updates
- Opportunity additions
- Opportunity analysis
- Strands agent use
- Draft generation
- Human review
- Opportunity deletion

The audit trail supports transparency, debugging, and responsible agent behaviour.

## Technology Stack

GrantPilot AI uses:

- Python 3.12
- Strands Agents SDK
- Amazon Bedrock
- Streamlit
- Boto3
- Pandas
- JSON-based local persistence

## Architecture

```text
Applicant
   |
   v
Streamlit User Interface
   |
   v
GrantPilot AI Orchestrator
   |
   +-- Applicant Profile Tool
   |
   +-- Opportunity Listing Tool
   |
   +-- Opportunity Evaluation Tool
   |
   +-- Application Planning Tool
   |
   v
Strands Agents SDK
   |
   v
Amazon Bedrock Foundation Model
   |
   v
Recommendation and Action Plan
   |
   +-- Human Approval Gate
   |
   +-- Local JSON Storage
   |
   +-- Transparent Audit Trail
