# CX Automation Case Studies

This repository contains sanitized case studies of internal CX automation workflows and tools I designed or built around AI-powered support systems, quality monitoring, expert feedback, and content intelligence.

The original projects were created in a proprietary environment, so these writeups focus on workflow design, architecture, problem-solving approach, and business impact rather than exposing internal data, code, or infrastructure.

These case studies show how I approach internal tooling: start from a real operational problem, design a workflow people can actually use, structure the data behind it, and build a simple interface for review and follow-up.

The original tools were built for CX automation around AI-powered support systems, but the same patterns apply to other internal workflows where teams need to capture feedback, monitor issues, and prioritize improvements.

## Sanitized internal case studies

### Expert Feedback Workflow

A human-in-the-loop workflow for capturing expert feedback on AI bot responses, classifying issues with lightweight codes, storing structured feedback, and connecting that feedback to existing bot interaction data for review.

This case study focuses on workflow design, feedback taxonomy and capture, data structure, and operational improvement loops.

[Read case study](case-studies/expert-feedback-workflow.md)

### Content Intelligence Dashboard

A Streamlit-based internal dashboard for centralizing AI support bot quality issues, content gaps, expert feedback, and recurring failure patterns into an actionable review workflow.

This case study focuses on dashboard design, issue triage, BigQuery-backed analytics, and content/prompt improvement workflows.

[Read case study](case-studies/content-intelligence-dashboard.md)

### FAQ Processor for Batch AI Assistant Evaluation

A Streamlit-based tool for batch-testing FAQ-style questions across multiple AI assistants.

The tool helped compare different assistants, prompt versions, and test environments without manually copying the same questions into several bots one by one.

This case study focuses on repeatable AI assistant testing, batch evaluation, structured result exports, and practical support for prompt/content review.

[Read case study](case-studies/faq-processor-batch-evaluation.md)


