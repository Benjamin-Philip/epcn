---
title: Exploring the Performance Characteristics of Nx 
author: Benjamin Philip
---

# Description

The Nx project brings Elixir to the domain of AI & ML. It makes a very large
promise: to leverage the BEAM in ML workflows, enabling us to run ML models
concurrently, distributed over multiple nodes, as well as partitioned across
several GPUs.

Closer inspection reveals that Nx is walking a tightrope: its computations are
powered by NIFs, whose scheduling is a tricky business, and GPUs, which support
a very small number of parallel processes. This raises the question: how is Nx
providing the high throughput that it boasts of?

Nx answers this question with "Servings" and "Batches", ways to batch requests
together to reduce and distribute the calls to the NIF and GPU. But how exactly
does that work? What trade-offs are we making by batching requests?

In this talk we will examine Nx's Servings, how it addresses the problem of
scheduling, the trade-offs and the performance characteristics of its approach,
as well as what are the other constraints when running an ML service.
    
# Session Format

In Person

# Key takeaways for the audience

In this talk you will learn:

- What are the problems to keep in mind when running an ML service
- How Nx addresses those problems
- What are the trade-offs made in, and caveats to its approach

# Target audience

This talk is targeted at people interested in:

- Using Nx in production
- The inner workings of Nx
- The general state of ML in the Elixir Ecosystem

# Level

Intermediate

# Which three words would best sum up your talk?

elixir-nx, Machine Learning, Performance
