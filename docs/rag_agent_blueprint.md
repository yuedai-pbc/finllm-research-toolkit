# RAG and Agent Workflow Blueprint for Economic Research

## Research Motivation

Financial and macroeconomic research often requires combining heterogeneous sources: central bank reports, financial statements, policy speeches, market data notes, academic papers, and internal research memos. Large language models can improve productivity, but only when the workflow is evidence-grounded, auditable, and structured.

This blueprint separates the workflow into retrieval, reasoning, drafting, and verification stages.

## 1. Source Layer

Recommended public-source categories:

- Central bank reports and speeches.
- Policy papers and working papers.
- Public financial disclosures.
- Academic abstracts and metadata.
- Market commentary with public redistribution rights.
- Public macroeconomic data dictionaries.

Do not include restricted, confidential, or copyrighted full-text materials unless redistribution is explicitly permitted.

## 2. Retrieval Layer

Core components:

- Document parser for PDF, HTML, Word, and Markdown.
- Metadata normalization, including date, author, institution, region, and topic.
- Chunking strategy by section, paragraph, or table.
- Embedding index for semantic retrieval.
- Keyword index for exact matching of policy terms, indicators, and institutions.

Recommended retrieval checks:

- Return source title, date, and section with each answer.
- Use hybrid retrieval for policy documents, because exact terminology matters.
- Avoid unsupported synthesis when retrieved evidence is weak.

## 3. Research Agent Layer

Possible agents:

- Literature mapper: classifies papers by task, data, model, and contribution.
- Policy scanner: extracts themes from public central bank materials.
- Macro memo assistant: drafts structured research notes with citations.
- Data dictionary assistant: maps indicators, source frequency, and limitations.
- Quality-control agent: checks citations, unsupported claims, and factual consistency.

## 4. Output Layer

Recommended outputs:

- Research memo.
- Literature table.
- Policy comparison matrix.
- Risk assessment note.
- Reproducible evidence log.
- Draft report outline.

## 5. Evaluation Layer

Evaluate outputs using:

- Evidence grounding.
- Citation correctness.
- Financial and macroeconomic accuracy.
- Robustness to ambiguous prompts.
- Transparency of assumptions.
- Reproducibility of retrieved sources.
