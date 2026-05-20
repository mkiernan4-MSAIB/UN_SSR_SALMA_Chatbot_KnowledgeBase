# UN SSR SALMA Chatbot Knowledge Base

This repository contains the data pipelines, document corpus structures, and agent frameworks powering an AI-driven knowledge system for United Nations Security Sector Reform (SSR).

At its core, this project transforms 20–25 years of UN SSR documentation into a structured, searchable, retrieval-grounded knowledge base that supports rapid generation of briefs, analysis, and decision-support outputs for SSR practitioners.

## Problem Statement

UN SSR teams face a persistent challenge: critical knowledge is distributed across decades of Secretary-General reports, policy documents, and country-level materials. Manual synthesis for reports and briefs is slow, inconsistent, and difficult to scale.

This project addresses that gap by structuring SSR knowledge into a system that enables fast, reliable, and reproducible analysis.

## Project Objectives

- Build a structured SSR document corpus with strong metadata, taxonomy, and traceability.
- Enable retrieval-augmented generation (RAG) using curated UN sources.
- Ensure all outputs are:
  - Grounded in authoritative documents
  - Consistent across use cases
  - Transparent and auditable
- Support generation of:
  - Country briefs
  - Analytical reports
  - Policy guidance
  - Talking points and decision-support artifacts

## What Is Security Sector Reform (SSR)?

Security Sector Reform is a UN-supported process aimed at helping states develop effective, accountable, and inclusive security institutions that serve citizens and uphold the rule of law.

SSR encompasses institutions such as:

- Armed forces
- Police and border services
- Justice and oversight bodies

SSR is recognized by the UN as a core component of peacebuilding, conflict prevention, and sustainable development.

## Repository Scope

This repository focuses on the data and knowledge layer:

1. **Corpus & Taxonomy**
   - Structured SSR document libraries, including:
     - Security Council resolutions
     - Secretary-General reports
     - Integrated Technical Guidance Notes (ITGNs)
     - CROSSROADS guidance modules
     - Country-specific SSR materials

2. **Knowledge Engineering**
   - Document normalization (PDF/DOCX → Markdown)
   - Metadata extraction and tagging
   - Deterministic chunking strategies for large policy documents
   - Source traceability linking each chunk to originating documents

3. **AI / Agent Framework**
   - Retrieval-augmented generation (RAG) pipelines
   - Copilot Studio / Teams integration patterns
   - Prompt discipline and grounding rules (source precedence, no hallucination)

4. **Output Templates**
   - Standardized formats for:
     - Briefs
     - Analytical outputs
     - Guidance modules
     - Talking points

## System Design Principles

- **Deterministic:** Reproducible outputs based strictly on source documents
- **Traceable:** Every output can be linked to underlying document(s)
- **Structured (not semantic guesswork):** Taxonomy-first design over free-form AI
- **Secure-by-design:** Supports evolution from open-source data to controlled enterprise knowledge
- **Grounded AI only:** No hallucinated or unverified content

## High-Level Architecture

- **Knowledge Layer:** Curated SSR documents (SharePoint / Markdown corpus)
- **Retrieval Layer:** Indexed document chunks with metadata
- **Agent Layer:** Copilot / AI agents with strict grounding rules
- **Interface Layer:**
  - Microsoft Teams (Q&A, briefs)
  - Copilot Chat (long-form analysis)

## Use Cases

- Rapid generation of country SSR briefs
- Cross-country comparative analysis
- Drafting UN-style reports and talking points
- Supporting policy development and planning
- Structured knowledge retrieval for field teams

## Project Status

- ✅ Corpus structuring and taxonomy design
- ✅ Knowledge base normalization pipeline
- ✅ Initial AI agent prototype (open-source data only)
- 🔄 Expansion to controlled datasets and enterprise deployment

## Why This Matters

Security Sector Reform sits at the intersection of peacekeeping, governance, human rights, and development. Yet the underlying knowledge base is fragmented and underutilized.

This repository demonstrates how AI plus structured knowledge engineering can unlock decades of institutional learning and make it actionable in real time.

## Future Work

- Expanded corpus coverage across SSR missions
- Integration of restricted/internal UN datasets (Phase 2)
- Advanced evaluation metrics for grounded AI outputs
- Automation of corpus updates and validation pipelines

## License and Usage

This project currently uses publicly available UN materials.
Future versions may include restricted data and require appropriate access controls.

## References

- United Nations: https://www.un.org/
- UN Peacekeeping / peace mission resources: https://peacekeeping.un.org/
