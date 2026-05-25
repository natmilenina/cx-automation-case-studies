# CX Automation Case Studies

This repository contains sanitized case studies of internal CX automation workflows and tools I designed or built around AI-powered support systems, quality monitoring, expert feedback, and content intelligence.

The original projects were created in a proprietary environment, so these writeups focus on workflow design, architecture, problem-solving approach, and business impact rather than exposing internal data, code, or infrastructure.

## What this portfolio shows

- Designing workflows around LLM-powered systems
- Turning messy human feedback into structured review data
- Building dashboards for quality monitoring and issue triage
- Prototyping internal tools with Python and Streamlit
- Working with operational data from sources such as BigQuery
- Supporting prompt, content, and process improvements through structured feedback loops

## Sanitized internal case studies

### Expert Feedback Workflow

A human-in-the-loop workflow for capturing expert feedback on AI bot responses, classifying issues with lightweight codes, storing structured feedback, and connecting that feedback to existing bot interaction data for review.

This case study focuses on workflow design, feedback taxonomy, data structure, and operational improvement loops.

[Read case study](case-studies/expert-feedback-workflow.md)

### Content Intelligence Dashboard

A Streamlit-based internal dashboard for centralizing AI support bot quality issues, content gaps, expert feedback, and recurring failure patterns into an actionable review workflow.

This case study focuses on dashboard design, issue triage, BigQuery-backed analytics, and content/prompt improvement workflows.

[Read case study](case-studies/content-intelligence-dashboard.md)

## Working approach

These case studies show how I approach internal tooling: start from a real operational problem, design a workflow people can actually use, structure the data behind it, and build a simple interface for review and follow-up.

The original tools were built for CX automation around AI-powered support systems, but the same patterns apply to other internal workflows where teams need to capture feedback, monitor issues, and prioritize improvements.

## Public demos

### Outlier Detection Workflow

A Streamlit app for detecting unusual patterns in operational/support-style data and surfacing records that may need human review.

This project demonstrates:
- anomaly/outlier detection logic
- operational monitoring thinking
- Streamlit dashboarding
- transforming raw data into reviewable signals

Links:
- [Live app](https://ai-support-outlier-monitoring.streamlit.app/)
- [GitHub repo](https://github.com/natmilenina/ai-support-outlier-monitoring/)

### RAG Playground

A Streamlit app for experimenting with retrieval-augmented generation workflows, retrieval quality, source-grounded answers, and prompt behavior.

This project demonstrates:
- RAG workflow design
- LLM API integration
- prompt testing
- retrieval debugging
- answer quality evaluation

Links:
- [Live app](https://compare-rag-configurations.streamlit.app/)
- GitHub repo: [add link]

