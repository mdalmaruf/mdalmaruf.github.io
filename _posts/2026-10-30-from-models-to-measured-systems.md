---
title: "From Models to Measured Systems: A Practical View of Embedded AI Research"
date: 2026-10-30
permalink: /posts/2026/10/from-models-to-measured-systems/
excerpt: "Reliable embedded AI begins when a promising model meets the timing, energy, safety, and maintenance constraints of a physical system."
tags:
  - Embedded AI
  - Cyber-Physical Systems
  - Edge Computing
  - Dependable Systems
---

Machine-learning research often begins with a model and a benchmark. Embedded-systems research begins with a different question: what must remain true when that model becomes part of a physical system?

An embedded AI component rarely operates in isolation. It shares limited compute, memory, energy, and network resources with sensing, control, communication, and safety functions. A model that is accurate in a notebook may miss a deadline on a target device. A fast inference pipeline may become unreliable when the sensor distribution changes. A software update that improves one component may introduce risk elsewhere in the system.

This is why I view embedded AI as a systems problem rather than only a model-design problem.

## Start with constraints, not only accuracy

Accuracy remains important, but it is one measure among several. Timing behavior, memory use, energy consumption, communication delay, fault response, and updateability all influence whether an intelligent component is suitable for deployment.

The practical research question is therefore multi-dimensional: how can we preserve useful model performance while respecting the constraints of the platform and the responsibilities of the full system?

That framing leads naturally to techniques such as model partitioning, resource-aware scheduling, edge–cloud task offloading, and runtime monitoring. It also makes trade-offs explicit. Moving part of a workload to an edge server may reduce device computation, for example, but add network uncertainty. A smaller model may improve latency while weakening detection performance. The right design depends on measurable system requirements.

## Build evidence on representative platforms

Simulation and offline analysis are valuable, but dependable systems need evidence closer to deployment. Hardware-in-the-loop and software-in-the-loop testbeds allow researchers to observe timing, failures, communication effects, and recovery behavior under controlled conditions.

At the NEST Research Lab, this model–build–measure cycle connects methods to physical platforms. The goal is not to add hardware for its own sake. It is to discover the gap between an algorithm's assumptions and the environment in which it must operate.

Representative evaluation also improves reproducibility. A well-described workload, platform, and test procedure can reveal why a method succeeds, where it fails, and whether another team can expect similar behavior.

## Treat software evolution as part of the research problem

Embedded systems often remain in service for years. Their software must be understood, tested, updated, and certified long after the first deployment. For that reason, software reuse and DevOps belong beside model optimization and runtime assurance.

Feature discovery can help engineers understand legacy code and identify reusable functionality. Structured testing can connect a change to the requirements and hardware it may affect. Carefully designed CI/CD pipelines can make assurance evidence part of the delivery process instead of an afterthought.

This is the motivation behind research directions such as FeaMod and ESOps: intelligent tooling should help engineers build software that is not only capable today, but also maintainable and trustworthy tomorrow.

## A useful definition of progress

For embedded AI, progress is more than a higher score on a single dataset. It is a clearer account of constraints, a method that can be implemented, evidence gathered on a representative system, and an engineering path from prototype to sustained use.

That combination—models, software, hardware, and measurement—is where embedded intelligence becomes dependable enough for the physical world.

*Explore related work on the [NEST Research Lab website](https://nestresearchlab.ca/) or browse my [publication list](/publications/).*
