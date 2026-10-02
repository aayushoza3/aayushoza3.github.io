---
layout: page
title: Specification Preservation in LLM-Orchestrated Systems
description: Does a guarantee on a tool survive when an LLM calls it?
importance: 1
category: research
---

When an LLM orchestrator invokes a trained classifier as a tool, the classifier may satisfy a specification that the overall system does not. This project studies that question using fairness as a measurable instance of a specification.

The setup has three components: an LLM orchestrator, a tool protocol (the Model Context Protocol), and a classifier tool. A monitor sits outside the decision path and compares the fairness of the tool's output with the fairness of the system's final decision. Lending is the application domain, because fair lending law provides an externally grounded property to check.

This is ongoing work in the Laboratory for Software Design at Tulane University.
