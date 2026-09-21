---
title: Citation Network Analysis Toolkit
status: Complete
year: 2023
tags: [graph analysis, bibliometrics, Python]
github: https://github.com/yourusername/citation-toolkit
---

A Python library for constructing and analyzing citation networks from structured bibliographic data. Useful for studying the diffusion of ideas across disciplines and identifying influential work that bridges communities.

## Features

- Parse and normalize records from arXiv, CrossRef, and Semantic Scholar
- Build directed citation graphs with rich metadata on nodes and edges
- Community detection and influence centrality measures
- Export to standard graph formats (GraphML, GEXFfor Gephi)

## Usage

Designed for researchers without a strong graph-theory background. The API is deliberately high-level: you load a set of papers, call `build_network()`, and get back a graph object ready for analysis.

## Publication

Results from this work are described in the paper *Bridging Communities: Cross-disciplinary Citation Patterns in Machine Learning* (see Publications).
