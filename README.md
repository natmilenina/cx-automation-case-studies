# CX Automation Case Studies

**Operating loop:**
real support conversations → AI assistant answer review → expert feedback → dashboard triage → content / prompt / routing / escalation / product follow-up → monitoring and retesting

This repository contains sanitized case studies of internal CX automation workflows and tools I designed or built around AI-powered support systems, quality monitoring, expert feedback, and content intelligence.

The original projects were created in a proprietary environment, so these writeups focus on workflow design, architecture, problem-solving approach, and business impact rather than exposing internal data, code, or infrastructure.

These case studies show how I approach internal tooling: start from a real operational problem, design a workflow people can actually use, structure the data behind it, and build a simple review layer that helps teams decide what to fix next.

The original tools were built for CX automation around AI-powered support systems, but the same patterns apply to other internal workflows where teams need to capture feedback, monitor issues, and prioritize improvements.

## System map

1. Capture support signals
2. Evaluate AI answers
3. Collect expert feedback
4. Centralize review
5. Prioritize fixes
6. Monitor regressions and quality shifts

## Projects in the system

| System layer | Project | What it does |
|---|---|---|
| Evaluation | FAQ Processor | Batch-tests questions across assistants / prompt versions |
| Human review | Expert Feedback Workflow | Lets experts flag bot issues in the tool they already use |
| Triage | Content Intelligence Dashboard | Centralizes issues, knowledge gaps, feedback, and recurring query patterns |
| Monitoring | Analytics Monitoring | Detects unusual shifts in support conversation patterns |

## Live demos

- Content Intelligence Dashboard: [Streamlit app](https://content-intelligence-dashboard-demo.streamlit.app/)
- Analytics Monitoring: [Streamlit app](https://ai-support-outlier-monitoring.streamlit.app)


## Sanitized internal case studies

### FAQ Processor for Batch AI Assistant Evaluation

A Streamlit-based tool for batch-testing FAQ-style questions across multiple AI assistants.

The tool helped compare different assistants, prompt versions, and test environments without manually copying the same questions into several bots one by one.

This case study focuses on repeatable AI assistant testing, batch evaluation, structured result exports, and practical support for prompt/content review.

[Read case study](case-studies/faq-processor-batch-evaluation.md)

### Expert Feedback Workflow

A human-in-the-loop workflow for capturing expert feedback on AI bot responses, classifying issues with lightweight codes, storing structured feedback, and connecting that feedback to existing bot interaction data for review.

This case study focuses on workflow design, feedback taxonomy and capture, data structure, and operational improvement loops.

[Read case study](case-studies/expert-feedback-workflow.md)

### Content Intelligence Dashboard

A Streamlit-based internal dashboard for centralizing AI support bot quality issues, content gaps, expert feedback, and recurring failure patterns into an actionable review workflow.

This case study focuses on dashboard design, issue triage, BigQuery-backed analytics, and content/prompt improvement workflows.

[View Streamlit dashboard demo](https://content-intelligence-dashboard-demo.streamlit.app/)

[Read case study](case-studies/content-intelligence-dashboard.md)

[View demo repo](https://github.com/natmilenina/content-intelligence-dashboard-demo/)

### Analytics Monitoring

An automated monitoring workflow for detecting unusual changes in AI support conversation patterns, surfacing affected user questions, and generating AI-assisted summaries to speed up investigation and prioritisation.

This case study focuses on support analytics, anomaly detection, quality monitoring, and proactive AI support improvement workflows.

[View synthetic data demo](https://ai-support-outlier-monitoring.streamlit.app)


## Tech and workflow areas

- Python
- Streamlit
- BigQuery
- GCP
- Telegram Bot API
- Google Dialogflow CX
- Mintlify Assistant API
- CSV/JSON-based review workflows
- Human-in-the-loop feedback
- AI bot quality review
- Batch testing and comparison
- Content and prompt improvement workflows

