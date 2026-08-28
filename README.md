<div align="center">

#  Awesome Error Propagation in Agentic AI

*A curated collection of research papers, datasets, tools, implementations, and learning resources related to Error Propagation in Multi-Step Agentic AI Workflows for Research Automation.*

[![Awesome](https://awesome.re/badge.svg)](https://awesome.re)
[![Maintenance](https://img.shields.io/badge/Maintained%3F-yes-green.svg)](https://GitHub.com/Naereen/StrapDown.js/graphs/commit-activity)

</div>

---

##  Contents
- [Overview](#-overview)
- [AI-Assisted Research Paper](#-ai-assisted-research-paper)
- [Survey Papers](#-survey-papers)
- [Foundational Papers](#-foundational-papers)
- [Recent Research Papers](#-recent-research-papers)
- [Datasets](#-datasets)
- [Tools and Libraries](#-tools-and-libraries)
- [GitHub Implementations](#-github-implementations)
- [Tutorials](#-tutorials)
- [Citation Integrity Audit](#-citation-integrity-audit)

---

##  Overview
> **Error propagation** in Large Language Model (LLM) agents occurs when a single faulty reasoning step, hallucinated tool call, or misinterpreted context cascades through a multi-step workflow, ultimately derailing autonomous tasks. 

This repository systematically categorizes research on how these error cascades occur and curates the latest mitigation strategies—including uncertainty-aware denoising, reinforcement learning safeguards, and root-cause isolation frameworks. It serves as a verified knowledge base for developing reliable AI research automation.

---

##  AI-Assisted Research Paper
**Error Propagation in Multi-Step Agentic AI Workflows for Research Automation**
* [View Paper](paper/MNS2026003_Paper.pdf)
> *An AI-generated baseline research paper exploring error cascades, complete with a systematic citation integrity audit.*

---

##  Survey Papers

**Agentic AI for Scientific Discovery: A Survey of Progress, Challenges, and Future Directions**
Gridach, M., et al., 2025, arXiv
[arXiv:2503.08979](https://arxiv.org/abs/2503.08979)
> A comprehensive overview of agentic AI applications and existing challenges in research workflows.

**The Rise and Potential of Large Language Model Based Agents: A Survey**
Xi, Z., et al., 2023, arXiv
[arXiv:2309.07864](https://arxiv.org/abs/2309.07864)
> Traces the development of language agents from cognitive models to AI algorithms, providing a unified framework consisting of brain, perception, and action modules.

**A Survey on LLM-based Multi-Agent System: Recent Advances and New Frontiers in Application**
Chen, S., et al., 2024, arXiv
[arXiv:2412.17481](https://arxiv.org/abs/2412.17481)
> Explores the coordination of intelligent agents in complex task-solving scenarios and highlights challenges related to scaling multi-agent systems.

**A Comprehensive Survey of Hallucination in Large Language Models**
Various Authors, 2025, arXiv
[arXiv:2510.06265](https://arxiv.org/abs/2510.06265)
> Analyzes the root causes of intrinsic and extrinsic hallucinations across the LLM development lifecycle and evaluates current mitigation techniques.

**Multi-Agent Collaboration Mechanisms: A Survey of LLMs**
Various Authors, 2025, arXiv
[arXiv:2501.06322](https://arxiv.org/abs/2501.06322)
> Investigates how multiple LLM-based agents communicate, coordinate, and recover from cascading reasoning failures during collaborative automation tasks.

---

##  Foundational Papers

**Chain-of-Thought Prompting Elicits Reasoning in Large Language Models**
Wei, J., et al., 2022, NeurIPS
[arXiv:2201.11903](https://arxiv.org/abs/2201.11903)
> Introduced the fundamental concept of prompting LLMs to generate intermediate reasoning steps, which serves as the baseline for tracking where logical errors originate.

**ReAct: Synergizing Reasoning and Acting in Language Models**
Yao, S., et al., 2022, ICLR
[arXiv:2210.03629](https://arxiv.org/abs/2210.03629)
> Established the foundational paradigm of interleaving reasoning traces with external tool actions to reduce hallucinations and ground AI behavior.

**Toolformer: Language Models Can Teach Themselves to Use Tools**
Schick, T., et al., 2023, NeurIPS
[arXiv:2302.04761](https://arxiv.org/abs/2302.04761)
> Demonstrated how language models can autonomously integrate external APIs via self-supervised learning, highlighting potential points of failure during automated tool execution.

**Tree of Thoughts: Deliberate Problem Solving with Large Language Models**
Yao, S., et al., 2023, NeurIPS
[arXiv:2305.10601](https://arxiv.org/abs/2305.10601)
> Proposed an advanced reasoning framework that allows agents to explore multiple decision paths, self-evaluate, and gracefully backtrack from erroneous logical branches.

**Reflexion: Language Agents with Verbal Reinforcement Learning**
Shinn, N., et al., 2023, NeurIPS
[arXiv:2303.11366](https://arxiv.org/abs/2303.11366)
> Introduced a framework for agents to maintain episodic memory and reflect on past failures, providing a vital mechanism to break out of cascading error loops.

---

##  Recent Research Papers

**From Spark to Fire: Modeling and Mitigating Error Cascades in LLM-Based Multi-Agent Collaboration**
Xie, Y., et al., 2026, arXiv
[arXiv:2603.04474](https://arxiv.org/abs/2603.04474)
> Analyzes modeling errors and provides mitigation strategies for LLM collaborations.

**DenoiseFlow: Uncertainty-Aware Denoising for Reliable LLM Agentic Workflows**
Yan, Y., et al., 2026, arXiv
[arXiv:2603.00532](https://arxiv.org/abs/2603.00532)
> Introduces a closed-loop framework for progressive denoising across multi-step reasoning chains.

**RL-Guard: Rescuing LLM Agents from Pitfalls**
Yang, Y., 2026, OpenReview
[OpenReview Link](https://api.semanticscholar.org/graph/v1/paper/search?query=RL-Guard:+Rescuing+LLM+Agents+from+Pitfalls)
> Presents a reinforcement learning safeguard to proactively prevent cascading failures without halting progress.

**Where LLM Agents Fail and How They can Learn From Failures**
Zhu, K., et al., 2025, arXiv
[arXiv:2509.25370](https://doi.org/10.48550/arxiv.2509.25370)
> Proposes an AgentErrorTaxonomy and Debug framework to isolate root-cause errors and provide corrective feedback.

---

##  Datasets

| Dataset Name | Source | Application | Link |
| :--- | :--- | :--- | :--- |
| **GAIA** | Hugging Face | Evaluates how LLM agents handle cascading errors during multi-step tool interactions. | [Access](https://huggingface.co/datasets/gaia-benchmark/GAIA) |
| **SWE-bench** | Princeton NLP | Traces error propagation during autonomous code debugging and repository navigation. | [Access](https://huggingface.co/datasets/princeton-nlp/SWE-bench) |
| **WebArena** | CMU | Analyzes execution failures and error recovery in highly interactive web environments. | [Access](https://github.com/web-arena-x/webarena) |
| **AgentBench** | THUDM | Provides step-by-step telemetry of how LLMs fail across terminal and database tasks. | [Access](https://github.com/THUDM/AgentBench) |
| **ToolBench** | OpenBMB | Maps the anatomy of a failure chain when an agent attempts to chain multiple APIs together. | [Access](https://github.com/OpenBMB/ToolBench) |
| **Mind2Web** | OSU-NLP | Studies how early navigational mistakes on live websites snowball into complete task failure. | [Access](https://github.com/OSU-NLP-Group/Mind2Web) |

---

##  Tutorials and Learning Resources

**1. LLM Powered Autonomous Agents**
* **Source:** Lilian Weng (OpenAI Applied Research)
* **Link:** [View Post](https://lilianweng.github.io/posts/2023-06-23-agent/)
* **Purpose:** A highly authoritative and comprehensive architectural breakdown of agent memory, planning, and tool use, highlighting how poor planning leads to unrecoverable errors.

**2. Building Effective Agents**
* **Source:** Anthropic
* **Link:** [View Documentation](https://www.anthropic.com/research/building-effective-agents)
* **Purpose:** Official guidance and best practices for designing robust, production-ready agentic workflows that minimize hallucinations and handle failure modes gracefully.

**3. AI Agents in LangGraph**
* **Source:** DeepLearning.AI / LangChain
* **Link:** [View Course](https://www.deeplearning.ai/short-courses/ai-agents-in-langgraph/)
* **Purpose:** A structured, hands-on video course teaching developers how to build cyclical state machines that allow agents to pause, self-reflect, and recover from execution errors.

**4. Microsoft AutoGen Official Tutorials**
* **Source:** Microsoft
* **Link:** [View Tutorials](https://microsoft.github.io/autogen/docs/tutorial/introduction)
* **Purpose:** Step-by-step technical guides on how to orchestrate multi-agent conversations, implement human-in-the-loop safeguards, and debug collaborative AI workflows.

**5. Hugging Face Open-Source AI Agents Course**
* **Source:** Hugging Face
* **Link:** [View Course](https://huggingface.co/learn/agents-course/unit0/introduction)
* **Purpose:** An open educational resource covering the fundamentals of how LLMs interact with external environments, execute tool calls, and navigate logical reasoning challenges.

---

##  Citation Integrity Audit
**Lab 1: AI-Assisted Citation Integrity Audit**
* [View Audit](citation-audit/Lab1_MNS2026003_ChandraShekharSahu.pdf)
> *A systematic audit verifying the existence, metadata accuracy, and claim-support entailment of the AI-generated references in the baseline paper.*

---
