**Agentic AI & System Architecture**
*This section curates foundational literature addressing system architectures, physical bottlenecks, and the general deployment of agentic workflows in scientific discovery.*

* **[Agentic AI for Scientific Discovery: A Survey of Progress, Challenges, and Future Directions](https://arxiv.org/abs/2503.08979)** - Gridach, M., et al. (2025). Investigates the deployment of agentic workflows across chemistry, biology, and materials science for tasks like literature synthesis and hypothesis testing. It highlights critical risks, including dual-use concerns and the danger of hallucinated scientific facts.
*BibTeX:* `@article{gridach2025agentic, title={Agentic AI for Scientific Discovery: A Survey of Progress, Challenges, and Future Directions}, author={Gridach, M. and Nanavati, J. and Zine El Abidine, K. and Mendes, L. and Mack, C.}, journal={arXiv preprint arXiv:2503.08979}, year={2025}}`


* **[A CPU-Centric Perspective on Agentic AI](https://www.google.com/search?q=https://doi.org/10.48550/arXiv.2511.00739)** - Raj, R., Wang, H., & Krishna, T. (2025). Analyzes system bottlenecks inherent in agentic workloads. The paper outlines how the repetitive nature of agentic flows and heavy reliance on CPU-centric tools (like Python interpreters) create significant latency and energy challenges.
*BibTeX:* `@article{raj2025cpu, title={A CPU-Centric Perspective on Agentic AI}, author={Raj, R. and Wang, H. and Krishna, T.}, journal={arXiv preprint arXiv:2511.00739}, year={2025}}`



**Error Cascades & Consensus Dynamics**
*Papers in this category explore the mechanisms of how minor semantic ambiguities in early reasoning steps compound laterally and chronologically into systemic failures.*

* **[From Spark to Fire: Modeling and Mitigating Error Cascades in LLM-Based Multi-Agent Collaboration](https://arxiv.org/abs/2603.04474)** - Xie, Y., et al. (2026). Characterizes error propagation in multi-agent environments as an evolutionary trajectory where local deviations solidify into a collective "false consensus". It explores how consensus inertia cements errors into system memory.
*BibTeX:* `@article{xie2026spark, title={From Spark to Fire: Modeling and Mitigating Error Cascades in LLM-Based Multi-Agent Collaboration}, author={Xie, Y. and Zhu, C. and Zhang, X. and Zhu, T. and Ye, D. and Qi, M. and Chen, H. and Zhou, W.}, journal={arXiv preprint arXiv:2603.04474}, year={2026}}`


* **[Where LLM Agents Fail and How They can Learn From Failures](https://www.google.com/search?q=https://doi.org/10.48550/arxiv.2509.25370)** - Zhu, K., et al. (2025). Introduces the AgentError Taxonomy to modularly classify failure modes across memory, planning, and action modules. It presents the Agent Debug framework to systematically isolate root causes and iteratively recover from mid-task failures.
*BibTeX:* `@article{zhu2025where, title={Where LLM Agents Fail and How They can Learn From Failures}, author={Zhu, K. and Liu, Z. and Li, B. and Tian, M. and Yang, Y. and Zhang, J. and Han, P. and Xie, Q. and Cui, F. and Zhang, W. and Ma, X. and Yu, X. and Ramesh, G. and Wu, J. and Liu, Z. and Lu, P. and Zou, J. and You, J.}, journal={arXiv preprint arXiv:2509.25370}, year={2025}}`



**Mitigation & Denoising Frameworks**
*This section focuses on active, closed-loop interventions and reinforcement learning safeguards designed to truncate error trajectories before total workflow failure.*

* **[DenoiseFlow: Uncertainty-Aware Denoising for Reliable LLM Agentic Workflows](https://arxiv.org/abs/2603.00532)** - Yan, Y., et al. (2026). Formalizes multi-step reasoning as a Noisy Markov Decision Process and introduces an active denoising framework. It utilizes empirical Monte Carlo sampling to estimate semantic uncertainty, allowing for surgical error correction without full workflow restarts.
*BibTeX:* `@article{yan2026denoiseflow, title={DenoiseFlow: Uncertainty-Aware Denoising for Reliable LLM Agentic Workflows}, author={Yan, Y. and Peng, J. and Li, S. and Li, C. and Shang, Y. and Deng, C. and Dai, R. and Zhao, Y. and Zhu, J. and Huang, Y.}, journal={arXiv preprint arXiv:2603.00532}, year={2026}}`


* **[RL-Guard: Rescuing LLM Agents from Pitfalls](https://openreview.net/)** - Yang, Y. (2026). Proposes a proactive safety reinforcement learning framework. It utilizes a critic to monitor trajectories, an actor to select corrective actions, and a risk-conditioned safety reward model to provide dynamic, step-level feedback during execution.
*BibTeX:* `@article{yang2026rlguard, title={RL-Guard: Rescuing LLM Agents from Pitfalls}, author={Yang, Y.}, journal={OpenReview}, year={2026}}`
