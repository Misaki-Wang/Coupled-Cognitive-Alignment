<div align="center">

<h1>Human Modeling Meets AI Metacognition</h1>

<hr>

<h2>Toward Coupled Cognitive Alignment for Interactive Agents</h2>

<p>Yaochen Wang<sup>1</sup>, Ming Li<sup>1,2</sup>, Xirui Li<sup>2</sup>, Tianyi Zhou<sup>1</sup></p>

<p><sup>1</sup>Mohamed bin Zayed University of Artificial Intelligence &nbsp;&nbsp; <sup>2</sup>University of Maryland</p>

</div>

The paper introduces **Coupled Cognitive Alignment (CCA)**, a research framework for building interactive AI agents that do more than produce correct answers. CCA argues that agents should decide *how to interact* by jointly reasoning about:

- what the human likely needs, knows, intends, trusts, or misunderstands;
- what the AI system can reliably know, do, verify, or risk;
- whether the next best action is to answer, ask, explain, retrieve evidence, defer, or escalate.

## Paper

- [Coupled-Cognitive-Alignment.pdf](./Coupled-Cognitive-Alignment.pdf)

## Core Idea

Many AI failures in human workflows are not just wrong outputs. They are wrong interaction choices. For example, an AI tutor may give a fully correct solution when a student actually needs a hint or a diagnostic question.

CCA frames this as an alignment problem at the **interaction-policy level**. Instead of optimizing only for response quality, an agent should align its next action with both:

1. **Human modeling**: an uncertainty-aware estimate of the user's latent cognitive state, such as goals, knowledge, preferences, trust, uncertainty, cognitive load, and reliance.
2. **AI metacognition**: an estimate of the agent's own uncertainty, capability boundaries, reliability, failure modes, information needs, and risks.

The paper proposes combining these into a **Joint Epistemic State (JES)**, which guides the agent's interaction policy over time.

## Framework Components

- **Dynamic Cognitive State Modeling (DCSM)**: models the human's evolving latent state from partial observations.
- **Metacognitive Self Modeling (MSM)**: models the AI system's own uncertainty, limitations, reliability, and risk.
- **Joint Epistemic State (JES)**: couples the human-side and AI-side beliefs into a decision-relevant state for policy selection.
- **JES-conditioned interaction policy**: selects whether the agent should answer directly, ask for clarification, explain uncertainty, retrieve evidence, decompose the task, defer, or escalate.
- **Recursive coupled update**: updates the joint state after each human response and new evidence from the interaction.

## Application Areas

The paper discusses CCA in high-stakes and long-horizon settings, including:

- education and tutoring;
- clinical and healthcare decision support;
- AI companions and mental health support;
- legal, financial, and organizational decision support;
- software engineering and scientific assistance;
- human-AI agent teaming.

## Research Challenges

The paper highlights several open problems:

- learning from sparse and ambiguous signals about latent human and agent states;
- evaluating interaction policies rather than only final answer accuracy;
- communicating uncertainty in ways that are useful for different users and contexts;
- designing governance boundaries for privacy, manipulation risk, autonomy, and deferral;
- building benchmarks for multi-turn, intervention-sensitive human-AI interaction.

## Status

This repository currently contains the paper PDF. The paper is a position paper and does not include an implemented system or released code.
