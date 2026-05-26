# FAQ Processor for Batch AI Assistant Evaluation

## Overview

Designed and built an internal Streamlit tool for batch-testing FAQ-style questions across multiple AI assistants.

The tool allows the team to upload a CSV of questions, select one or more processors, run the same questions through different assistants, and download the results for review.

It was created for a CX automation context where testing individual questions manually was too slow, especially when comparing different bot versions, prompts, or assistant configurations.

## Problem

Manual testing was fine for checking a few bot answers, but it quickly became inefficient for larger FAQ batches.

When the team needed to compare different assistants, prompt versions, or knowledge base set ups, the same questions had to be copied into multiple places and the answers collected manually. That made the process slow, tedious, and bot answer quality evaluations became a bottleneck.

The goal was to create a simple way to run the same question set through selected assistants and get all answers, errors, and metadata back in one structured output, available for export and sharing.


## Solution

Built a Streamlit batch-processing tool that takes a CSV of questions and sends each question to selected AI assistants.

The app returns a structured results file containing the original question, metadata from the input CSV, each selected assistant’s answer, success/error status, and timestamps.

This made it easier to compare responses side by side and create review datasets for prompt, content, or bot configuration improvements.

## Core functionality

- Password-protected internal access
- CSV template download for preparing question batches
- CSV upload with required `id_number` and `question` fields
- Optional metadata columns (such as category, theme, source etc)
- Processor selection for testing one or more assistants
- Support for multiple assistant backends, including Mintlify AI Assistant API and Dialogflow CX agents
- Batch processing with progress tracking
- Rate-limit handling with delay between requests
- Retry logic for temporary API failures
- Summary metrics showing successful responses per processor
- Results preview inside the app
- Downloadable results in CSV and JSON formats

## Workflow

1. User selects which AI assistants/processors to test.
2. User downloads or prepares a CSV of FAQ-style questions.
3. User uploads the CSV into the app.
4. The app validates that required columns are present.
5. Each question is sent to the selected processors.
6. Answers, success statuses, errors, and timestamps are collected.
7. Results are shown in the app for quick review.
8. The full output can be downloaded as CSV or JSON for deeper analysis.

## System flow

```mermaid
flowchart LR
    A["CSV of FAQ questions"] --> B["Streamlit app"]
    B --> C["Processor selection"]

    C --> D["Mintlify Assistant API"]
    C --> E["Dialogflow CX agent 1"]
    C --> F["Dialogflow CX agent 2"]
    C --> G["Testing / Staging agents"]

    D --> H["Structured results"]
    E --> H
    F --> H
    G --> H

    H --> I["Results preview"]
    H --> J["CSV download"]
    H --> K["JSON download"]
    H --> L["Manual / expert review"]
