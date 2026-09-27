# BDI-Based Explainable AI for Architectural Design

Bachelor's project by Rakan Al-Swayyed · Universität Hildesheim · 2020

This research project explored how a belief-desire-intention (BDI) agent architecture can make case-based architectural design recommendations easier to understand. It extended the MetisCBR research framework with agents that organize and generate explanations for floor-plan retrieval results.

## Research question

**How can BDI agents be integrated as an explanation component so that they support architects in early design phases?**

The aim was to complement retrieved similar floor plans with explanations that help a user understand the recommendation and recognize when supplied design information is insufficient.

## Explanation model

The project used three complementary explanation patterns:

| Pattern | User-facing purpose |
| --- | --- |
| **Transparency** | Explains how the system reached a result. |
| **Justification** | Explains why a result is suitable. |
| **Relevance** | Explains why available query information cannot support a dependable positive explanation. |

The prototype covered room-graph, adjacency, accessibility, and full-graph floor-plan fingerprints.

## Agent workflow

The BDI design separates responsibilities across three cooperating agents:

1. **Belief** receives a request, identifies the applicable fingerprint, and returns the completed explanation.
2. **Desire** identifies relevant explanation patterns and coordinates completion.
3. **Intention** applies the selected plan to generate the explanation text for the query and retrieved results.

This structure linked case-based retrieval with a traceable, user-facing explanation workflow.

## Historical evaluation

The 2020 thesis evaluated 48 queries across four fingerprint types. In that controlled study, the reported aggregate outcomes were 43% Justification, 40% combined Justification and Transparency, 16% Transparency, and 1% Relevance. These are historical research findings from the thesis, not claims of present-day system performance.

## Technical approach

The project used Java, JADE agents, myCBR, graph matching, Maven, and IntelliJ IDEA. It built on the existing MetisCBR framework and related research software; it does not claim sole authorship of that underlying platform.

## Preservation status

The project was recovered and checked in September 2026. All 140 Java source files in the main project compiled, a fresh Maven build succeeded, the backend and BDI agents initialized, and a focused relevance-explanation test passed. These checks establish partial recoverability, not complete end-to-end validation or production readiness.

## Repository scope

This public repository is a descriptive portfolio summary only. Source code, datasets, binaries, original project history, detailed technical documentation, and preservation archives remain in a separate private repository and are not published here.
