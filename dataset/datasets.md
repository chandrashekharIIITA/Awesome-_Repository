# Datasets

**1. GAIA (General AI Assistants Benchmark)**
* **Source:** Hugging Face / Meta AI & Yann LeCun's Research Group[cite: 1]
* **Description:** Rather than testing basic factual recall, GAIA acts as a rigorous stress test for autonomous systems. It consists of highly challenging, real-world questions that are conceptually straightforward for humans but notoriously difficult for current AI models. To find the correct answer, an agent must independently break down the core problem, browse the live web, select appropriate external tools, and reason through a lengthy sequence of steps without losing context.[cite: 1]
* **Application:** This benchmark is an excellent tool for researchers studying error cascades. Because the tasks require multiple sequential tool calls, you can trace the exact moment an agent makes a poor decision—such as misinterpreting a search result—and map how that single failure snowballs, eventually derailing the entire workflow.[cite: 1]
* **Link:** https://huggingface.co/datasets/gaia-benchmark/GAIA[cite: 1]

**2. SWE-bench: Can Language Models Resolve Real-World GitHub Issues?**
* **Source:** Princeton NLP[cite: 1]
* **Description:** SWE-bench goes far beyond static text evaluation by offering a massive collection of real, historical software engineering problems pulled directly from popular open-source Python repositories on GitHub. It challenges AI agents to read a user issue, autonomously navigate a complex, multi-file codebase, understand the broader context, and ultimately write a patch that successfully passes strict unit tests.[cite: 1]
* **Application:** Software engineering naturally requires long-horizon planning, making this dataset a goldmine for analyzing multi-step error propagation. Researchers use SWE-bench to observe how an AI's initial misunderstanding of a repository's architecture leads to compounding downstream errors, especially as the agent iteratively attempts to execute and debug the faulty code it just generated.[cite: 1]
* **Link:** https://huggingface.co/datasets/princeton-nlp/SWE-bench[cite: 1]

**3. WebArena: A Realistic Web Environment for Building Autonomous Agents**
* **Source:** Carnegie Mellon University (CMU)[cite: 1]
* **Description:** WebArena provides a fully interactive, simulated web environment that mirrors the complexity of the actual internet, complete with functional e-commerce platforms, forums, and content management systems. The dataset pairs this sandbox with hundreds of complex, intent-driven tasks that require an agent to actively navigate pages, interact with UI elements, and synthesize information just as a human web surfer would.[cite: 1]
* **Application:** Because the simulation is highly interactive and unforgiving of bad logic, it is perfectly suited for pinpointing execution failures. Researchers analyze the step-by-step interaction logs to understand how agents handle ambiguous web layouts, where they introduce critical pathing errors (like clicking the wrong navigation link), and whether they possess the self-correction capabilities needed to recover before the workflow fails completely.[cite: 1]
* **Link:** https://github.com/web-arena-x/webarena[cite: 1]
