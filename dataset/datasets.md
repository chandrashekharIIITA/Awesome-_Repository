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

**4. AgentBench: A Comprehensive Benchmark to Evaluate LLMs as Agents**
* **Source:** Tsinghua University (THUDM)
* **Description:** AgentBench is a massive, multi-modal benchmarking framework designed to evaluate how well Large Language Models function as autonomous agents across eight distinct interactive environments. Instead of simple question-answering, it forces the AI to interact with operating systems, databases, knowledge graphs, and simulated web shops. The dataset contains thousands of multi-turn interaction logs where an agent must issue commands, interpret system feedback, and decide on the next logical step. 
* **Application:** For researchers studying error propagation, this dataset provides raw, step-by-step telemetry of how LLMs fail in the wild. By analyzing the logs from the Operating System or Database environments, you can trace exactly when an agent misreads a terminal output, how it confidently proceeds with a flawed assumption, and why it ultimately fails to recover from cascading logic errors.
* **Link:** https://github.com/THUDM/AgentBench

**5. ToolBench: An Open Platform for Tool Learning**
* **Source:** OpenBMB / Tsinghua University
* **Description:** ToolBench is an extensive instruction-tuning dataset built to train and evaluate LLMs on using over 16,000 real-world REST APIs from RapidAPI. It features a novel decision-tree annotation method that captures not just the final answer, but the entire multi-step reasoning process, the specific API tool executed, and the raw execution results. The dataset encompasses both single-tool and highly complex multi-tool scenarios where the output of one API must be flawlessly fed into another.
* **Application:** This is a crucial resource for diagnosing "tool-use hallucinations." Researchers use ToolBench to identify where agentic workflows break down during API interactions—such as hallucinating a non-existent parameter, misformatting a JSON payload, or failing to understand a tool's error message. It allows developers to map the anatomy of a failure chain when an agent attempts to chain multiple APIs together.
* **Link:** https://github.com/OpenBMB/ToolBench

**6. Mind2Web: Towards a Generalist Agent for the Web**
* **Source:** Ohio State University NLP Group (OSU-NLP)
* **Description:** Mind2Web is a pioneering dataset developed to train and evaluate generalist web agents. It contains over 2,000 open-ended, multi-step tasks crowdsourced across 137 real-world websites spanning 31 different domains. It pairs raw and cleaned HTML documents with exact user action sequences (like clicking, typing, and selecting) required to complete complex objectives (e.g., booking a flight or buying a specific item) in non-simulated web environments.
* **Application:** Because the web is highly dynamic and chaotic, Mind2Web is perfect for studying robust error recovery. Researchers analyze this dataset to see how an agent's workflow derails when a webpage layout changes or a pop-up appears, providing insight into semantic ambiguity, context loss, and how early navigational mistakes snowball into complete task failure.
* **Link:** https://github.com/OSU-NLP-Group/Mind2Web
