---
layout: page
title: research
permalink: /research/
description: Software engineering for trustworthy and fair agentic AI systems.
nav: true
nav_order: 1
---

## Overview

Modern AI systems are rarely a single model. A large language model plans, calls tools, reads their outputs, and produces a final decision. Each tool may have been tested carefully on its own, but the system that a person actually interacts with is the composition. My research asks what happens to the guarantees of the parts when they are composed, and how software engineering techniques can make those guarantees explicit and checkable.

I work in the Laboratory for Software Design at Tulane University, advised by [Hridesh Rajan](https://hridesh.github.io).

## Research Interests

- **Agentic AI and AI decision making.** How LLM-based agents use tools and side models to reach decisions, and how to reason about the resulting behavior.
- **Algorithmic fairness.** Measuring and preserving group fairness properties in machine learning pipelines, with a focus on high-stakes domains such as lending.
- **Design by Contract for AI systems.** Writing specifications for the components of an AI system and checking them at the boundaries where components interact.
- **Software engineering for machine learning.** Testing, debugging, and replication of ML systems.

## Current Projects

### Specification preservation in LLM-orchestrated systems

When an LLM orchestrator invokes a trained classifier as a tool, the classifier may satisfy a specification that the overall system does not. I study this question using fairness as a measurable instance of a specification. The setup has three components: an LLM orchestrator, a tool protocol (the Model Context Protocol), and a classifier tool. A monitor sits outside the decision path and compares the fairness of the tool's output with the fairness of the system's final decision. Lending is the application domain, because fair lending law provides an externally grounded property to check.

### Fairness evaluation of ensemble classifiers on lending data

Building on prior work from the lab on fairness composition in ensemble machine learning, I evaluate ensemble classifiers across several public lending datasets, including HMDA mortgage data, Adult Census, Taiwan Credit, and German Credit. The goal is to understand how well fairness and accuracy tradeoffs reported on benchmark datasets carry over to realistic lending data.

### Contracts for agentic fairness

I am exploring a multi-agent design that combines Design by Contract with causal debugging, so that a violated fairness contract can be traced to the component responsible for it.

## Earlier Work

- **Replication of neural network repair.** I replicated the experiments of the IRepair paper (FSE 2025) on intent-aware repair of large language models.

## Publications

A full list is on the [publications page]({{ '/publications/' | relative_url }}).
