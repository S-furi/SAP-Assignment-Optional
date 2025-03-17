+++
title = "My First Presentation"
outputs = ["Reveal"]
+++

---

Contents:
- [Background](#background)
  - [Agents in Symbolic AI](#agents-in-symbolic-ai)
    - [Agents as String Manipulation Systems](#agents-as-string-manipulation-systems)
  - [Cognitive Agents](#cognitive-agents)
  - [Production Systems and Human Cognition](#production-systems-and-human-cognition)
    - [An Example: SOAR Architecture](#an-example-soar-architecture)
    - [*Memory*](#memory)
    - [*Grounding*](#grounding)
    - [*Decision Making*](#decision-making)
    - [Learning](#learning)
- [](#)

---

## Background

With the term **Language Agents**, we refer to an emerging class of AI systems that use Large
Language Models (LLM) to interact with the world, applying together current advancement in AI to the
existing field of agent design, offering benefits for both fields.

---

{{% section %}}
### Agents in Symbolic AI

The rise of Agents in symbolic AI comes from the concept of **Production Systems**:

> Production Systems generate a set of outcomes by iteratively applying rules

A production system basically consists of:

- A set of *rules*, each one specifying:
    - a *precondition*
    - an *action*

---

#### Agents as String Manipulation Systems

E. L. Post proposed thinking about arbitrary logical systems in terms of
production systems.

Later on, it will be shown to be equivalent to a simpler *string rewriting*
system of the form:

```math
XYZ \rightarrow XWZ
```

This lead to the definition of complex behaviours by means of simple
productions.

{{% /section %}}

---

### Cognitive Agents

---

### Production Systems and Human Cognition

AI community exploited some aspects of *"human cognition"* by means of
sophisticated production systems connected to external sensors, actuator and
knowledge bases. 

> **Cognitive Architectures**: agents that uses processes such as *perception*,
> *memory* and *planning* to archive complex behaviours.

---

{{% section %}}

#### An Example: SOAR Architecture
<img src="figures/The-Soar-cognitive-architecture.png">

------

#### *Memory*

<img src="figures/The-Soar-cognitive-architecture.png" width="500" >

- **Long Term Memories** (procedural, semantic, episodic)
- **Short Term Working Memory**

------

#### *Grounding*

<img src="figures/The-Soar-cognitive-architecture.png" width="500" >

- **Sensors** generates percepts
- **Actuators** allow physical interaction with environment

------

#### *Decision Making*

```mermaid
graph TD 
  in(["Input"])
  prop["Proposal and Evaluation"]
  act(["Action Selection"])
  out(["Output"])
  in --> prop
  prop --> act
  act --> Application
  Application --> out
  out --> in
```

---

#### Learning

<img src="figures/The-Soar-cognitive-architecture.png" width="500" >
---
{{% /section %}}


