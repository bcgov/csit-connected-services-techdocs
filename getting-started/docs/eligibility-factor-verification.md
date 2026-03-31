---
title: Eligibility Factor Verification (EFV) 
---
# Getting started with Connected Services

## Eligibility Factor Verification (EFV) 

### What it is 

_Eligibility Factor Verification_ (EFV) is the administrative process of confirming that the information provided by an applicant is accurate and meets the rules for a specific government benefit or service. 

It standardizes how programs verify deterministic facts such as income thresholds, residency status, or identity. 

EFV serves as the bridge between authoritative data and a program’s eligibility rules. It helps confirm deterministic facts like income thresholds, residency status, and identity. 

The EFV framework supports: 

- Connection to trusted and authoritative data sources 
- Reduction of manual interpretation and document review 
- Faster, more consistent decision support 
- A defensible evidence trail for explainability and audit 

### Who this is for 

EFV supports both those building eligibility systems and those responsible for program outcomes. 

**Primary audience**

- Developers building eligibility tools and integrations 
- Solution architects designing automated adjudication systems 

**Secondary audience**

- Product owners managing benefit programs 
- Program and policy leads defining eligibility criteria 
- Adjudicators and intake staff using decision-support tools 

### When to use Eligibility Factor Verification 

Use EFV when: 

- You need to confirm a specific, verifiable fact (e.g., “Is this person a B.C. resident?”) 
- You want to replace manual document collection and reviews with trusted automated data signals 
- You require a defensible audit trail explaining how a determination was reached 

EFV is best suited for deterministic checks. 

It should not be used for complex cases requiring significant human discretion or contextual judgment unless those patterns are clearly defined and governed. 

### How it works (high level) 

1. A program identifies the specific eligibility factors required (e.g., income, residency). 
2. The system connects to an Authoritative Data source. 
3. A verification check compares applicant information to the trusted dataset. 
4. The system returns a verification signal (e.g., Pass/Fail) along with metadata such as source and verification timestamp. 
5. Adjudicators use the signal to support automated approval or focus on exceptions requiring review. 

Verification is most effective when it reduces the need for applicants to upload scans or photographs of physical documents. 

### Where to go next 
<span style="color:red; font-weight:bold">TODO Add Links when available</span>

- Eligibility Factor Verification Standards 
- Authoritative Data Directory 
- Trust Metadata and Lineage Guidelines  