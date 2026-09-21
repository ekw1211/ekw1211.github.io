---
title: Semantic Search over Scientific Literature
status: Active
year: 2024
tags: [NLP, information retrieval, transformers]
github: https://github.com/yourusername/semantic-search
---

A retrieval system for scientific papers that goes beyond keyword matching. Given a natural-language query, the system returns documents ranked by semantic relevance using dense vector representations.

## Motivation

Existing literature search tools rely primarily on keyword overlap and citation graphs. This leaves a gap: papers that answer a question without using the question's vocabulary are systematically underweighted. The goal of this project is to close that gap for researchers working at the boundaries of established subfields.

## Approach

Queries and documents are encoded using a fine-tuned bi-encoder architecture. The index is built over a corpus of ~2M abstracts from open-access repositories. Retrieval latency is kept under 200ms via approximate nearest-neighbor search.

## Status

Actively developed. A web interface is available for beta testing. Feedback welcome.
