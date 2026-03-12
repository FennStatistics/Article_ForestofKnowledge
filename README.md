# Forests of Knowledge

Forests of Knowledge: Perceptions of the Forest in Literature Over Time is an interdisciplinary project that studies the forest as an epistemic and symbolic entity in literature and tracks how narrative and normative framings shift across history. The project uses LLMs and NLP to perform diachronic analysis on a machine-readable corpus, identifying long-term changes in cultural perception and ecological knowledge.

## Project Context

- Key Research Area: Languages of Knowledge (University of Freiburg)
- Proposal type: Networking Grant for Early-Career Researchers (2026)
- Proposal date: 15.01.2026

## Objectives

- Build a shared, open, machine-readable literary corpus focused on forest representations.
- Analyze temporal orders and normative understandings of forests, including potential signals of biodiversity loss in literary descriptions over time.
- Establish a stable interdisciplinary research network and prepare a major third‑party funding proposal.

## Methodology

- Diachronic analysis with NLP/LLMs using vector embeddings and prompt-based learning.
- Retrieval-Augmented Generation (RAG) to ground interpretations in specific retrieved passages.
- Sentiment and framing analysis to quantify emotional valence (threat vs. sanctuary) and classify themes (Utility, Recreation, Imagination).
- Statistical trend analysis to detect historical breaks and semantic continuities.

## Technical Implementation (Planned)

- Data sourcing: Automated collection from literary databases (e.g., Project Gutenberg) via controlled, policy-compliant workflows.
- Storage: Vector database (Supabase) for text and metadata.
- Processing: Embeddings via Qwen models and classification via BERT-based architectures.
- Interface: Web-based UI hosted through the University of Freiburg Rechenzentrum.

## Expected Innovation

The project introduces AI-driven, large-scale diachronic analysis to a field that is currently dominated by synchronic or qualitative approaches. It aims to operationalize “wide reading” by combining environmental humanities with computational statistics, enabling measurable comparisons of symbolic, narrative, and normative forest perceptions across centuries. The resulting corpus and annotation guidelines will provide reusable infrastructure for future environmental humanities research.

## Work Packages & Resourcing

- WP1: Consolidation of terminology, concepts, and corpus design.
- WP2: Automated scraping and initial database setup.
- WP3: Manual curation, annotation, and classification by a student assistant.
- WP4: University-wide expert workshop and start of a major grant proposal.

Personnel costs: €3,000 for a graduate student assistant (WHK) to support WP3, covering approximately 14–16 hours/month in 2026. All software development, programming, and technical infrastructure (RAG + database setup) are handled by the applicants.

## Team

- Dr. Julius Fenn (Department of Psychology): Computational modeling, statistics, NLP; technical execution and quantitative analysis.
- Dr. Finn Rehling (Chair of Nature Conservation and Landscape Ecology): Forest ecosystems and biodiversity; ecological framework and environmental contextualization.
- Juliane Amberger (Department of Scandinavian Studies): Narrative theory, cultural and literary history; corpus selection and qualitative interpretation.

## External Data Sources & Access Constraints (Internet Scan Summary)

- Project Gutenberg: The site is US-focused; non‑US users must check local copyright. Automated access to the main site can trigger IP blocks, and bulk downloading should use mirrors or offline catalogs instead of scraping the main site. What this means: we must verify copyright by jurisdiction, use mirrors/catalog dumps for bulk acquisition, and implement respectful rate limits.
- Wikimedia dumps (incl. Wikisource via Wikimedia Downloads): Wikimedia provides monthly dumps of all public wikis in XML and applies rate limits and per‑IP connection caps on the download servers. What this means: use official dumps rather than page‑by‑page scraping, and plan for large storage plus a repeatable import pipeline.
- RAG as a method: Retrieval‑augmented generation combines parametric LLMs with a non‑parametric dense vector index to ground outputs in retrieved evidence. What this means: we need a high‑quality vector index, provenance tracking, and retrieval evaluation alongside generation.

## To‑Do (Priority Steps)

1. Confirm copyright status per text and jurisdiction, starting with Project Gutenberg’s US‑public‑domain scope and any non‑US restrictions.
2. Decide primary corpus sources and acquisition method (mirrors/dumps vs. live scraping) and document compliance with each provider’s access policy.
3. Build the ingestion pipeline: download, normalize, de‑duplicate, and store raw texts plus metadata.
4. Define corpus schema and annotation guidelines (themes, temporal metadata, ecological concepts).
5. Implement embeddings + vector store indexing; version the embedding model and metadata schema.
6. Implement RAG retrieval: chunking strategy, top‑k retrieval, provenance logging, and retrieval evaluation.
7. Add NLP pipelines: sentiment, framing classification, topic modeling, diachronic trend detection.
8. Add regex/lexicon search utilities for targeted queries (e.g., species, exploitation metaphors, protection language).
9. Validate results with qualitative close reading and interdisciplinary review.
10. Prepare workshop materials and draft the major third‑party grant proposal.
