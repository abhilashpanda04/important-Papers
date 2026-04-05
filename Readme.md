# Important Papers in Large Language Models and AI

A curated collection of influential research papers in Machine Learning, Large Language Models, and AI — organized by topic. This list covers foundational work through to the latest developments in 2025-2026.

---

## Table of Contents

- [Foundation Models and Architecture](#foundation-models-and-architecture)
- [Attention and Efficiency](#attention-and-efficiency)
- [State Space Models and Alternatives to Transformers](#state-space-models-and-alternatives-to-transformers)
- [Reasoning and Chain-of-Thought](#reasoning-and-chain-of-thought)
- [Reinforcement Learning from Human Feedback (RLHF) and Alignment](#reinforcement-learning-from-human-feedback-rlhf-and-alignment)
- [Retrieval-Augmented Generation (RAG)](#retrieval-augmented-generation-rag)
- [AI Agents and Tool Use](#ai-agents-and-tool-use)
- [Fine-Tuning and Adaptation](#fine-tuning-and-adaptation)
- [Mixture of Experts (MoE)](#mixture-of-experts-moe)
- [Long Context and Memory](#long-context-and-memory)
- [Quantization and Compression](#quantization-and-compression)
- [Inference Optimization and Serving](#inference-optimization-and-serving)
- [Multimodal Models](#multimodal-models)
- [Code Generation](#code-generation)
- [Evaluation and Benchmarks](#evaluation-and-benchmarks)
- [Surveys](#surveys)
- [Diffusion and Image Generation](#diffusion-and-image-generation)

---

## Foundation Models and Architecture

| Title | Link | Notes |
|-------|------|-------|
| Attention Is All You Need | [arXiv:1706.03762](https://arxiv.org/abs/1706.03762) | The original Transformer paper that started it all |
| GPT-4 Technical Report | [arXiv:2303.08774](https://arxiv.org/abs/2303.08774) | OpenAI's multimodal flagship model |
| LLaMA: Open and Efficient Foundation Language Models | [arXiv:2302.13971](https://arxiv.org/abs/2302.13971) | Meta's foundational open-weight LLM |
| LLaMA 2: Open Foundation and Fine-Tuned Chat Models | [arXiv:2307.09288](https://arxiv.org/abs/2307.09288) | Scaled up LLaMA with RLHF chat variants |
| LLaMA 3.1: Herd of Models | [Meta AI](https://ai.meta.com/research/publications/the-llama-3-herd-of-models/) | 405B parameter open-weight model |
| Yi: Open Foundation Models by 01.AI | [arXiv:2403.04652](https://arxiv.org/abs/2403.04652) | High-quality bilingual foundation model |
| Gemma 2: Improving Open Language Models at a Practical Size | [arXiv:2408.00118](https://arxiv.org/abs/2408.00118) | Google's efficient open-weight models |
| Qwen2.5 Technical Report | [arXiv:2412.15115](https://arxiv.org/abs/2412.15115) | Alibaba's strong multilingual model family |
| DeepSeek-V3 Technical Report | [arXiv:2412.19437](https://arxiv.org/abs/2412.19437) | 671B MoE model trained on 14.8T tokens at remarkably low cost |
| Gemini: A Family of Highly Capable Multimodal Models | [arXiv:2312.11805](https://arxiv.org/abs/2312.11805) | Google's multimodal foundation model |
| Mistral 7B | [arXiv:2310.06825](https://arxiv.org/abs/2310.06825) | Punching above its weight with Sliding Window Attention and GQA |
| OLMo: Accelerating the Science of Language Models | [arXiv:2402.00838](https://arxiv.org/abs/2402.00838) | Fully open model: weights, data, training code, and evaluation |
| SmolLM2: When Smol Goes Big | [arXiv:2502.02737](https://arxiv.org/abs/2502.02737) | HuggingFace's strong small language models (135M to 1.7B) |

## Attention and Efficiency

| Title | Link | Notes |
|-------|------|-------|
| FlashAttention: Fast and Memory-Efficient Exact Attention with IO-Awareness | [arXiv:2205.14135](https://arxiv.org/abs/2205.14135) | IO-aware exact attention — now industry standard |
| FlashAttention-2: Faster Attention with Better Parallelism and Work Partitioning | [arXiv:2307.08691](https://arxiv.org/abs/2307.08691) | 2x speedup over FlashAttention |
| FlashAttention-3: Fast and Accurate Attention with Asynchrony and Low-precision | [arXiv:2407.08691](https://arxiv.org/abs/2407.08691) | Hopper GPU optimizations, FP8 support |
| GQA: Training Generalized Multi-Query Transformer Models from Multi-Head Checkpoints | [arXiv:2305.13245](https://arxiv.org/abs/2305.13245) | Grouped-Query Attention used in LLaMA 2/3, Mistral |
| Ring Attention with Blockwise Transformers for Near-Infinite Context | [arXiv:2310.01889](https://arxiv.org/abs/2310.01889) | Distributes attention across devices for near-infinite context |
| DeepSeek-V2: A Strong, Economical, and Efficient Mixture-of-Experts Language Model | [arXiv:2405.04434](https://arxiv.org/abs/2405.04434) | Multi-head Latent Attention (MLA) — compresses KV cache drastically |

## State Space Models and Alternatives to Transformers

| Title | Link | Notes |
|-------|------|-------|
| Mamba: Linear-Time Sequence Modeling with Selective State Spaces | [arXiv:2312.00752](https://arxiv.org/abs/2312.00752) | Selective SSM — linear-time alternative to Transformers |
| Mamba-2: Transformers are SSMs | [arXiv:2405.21060](https://arxiv.org/abs/2405.21060) | Shows Transformers and SSMs are duals via SSD framework |
| Jamba: A Hybrid Transformer-Mamba Language Model | [arXiv:2403.19887](https://arxiv.org/abs/2403.19887) | AI21's hybrid architecture combining both paradigms |
| RWKV: Reinventing RNNs for the Transformer Era | [arXiv:2305.13048](https://arxiv.org/abs/2305.13048) | Linear-complexity RNN that matches Transformer performance |
| Griffin: Mixing Gated Linear Recurrences with Local Attention for Efficient Language Models | [arXiv:2402.19427](https://arxiv.org/abs/2402.19427) | Google's hybrid recurrent + attention architecture |

## Reasoning and Chain-of-Thought

| Title | Link | Notes |
|-------|------|-------|
| Chain-of-Thought Prompting Elicits Reasoning in Large Language Models | [arXiv:2201.11903](https://arxiv.org/abs/2201.11903) | The foundational CoT paper by Google |
| Tree of Thoughts: Deliberate Problem Solving with Large Language Models | [arXiv:2305.10601](https://arxiv.org/abs/2305.10601) | Extends CoT into branching search trees |
| Self-Consistency Improves Chain of Thought Reasoning in Language Models | [arXiv:2203.11171](https://arxiv.org/abs/2203.11171) | Sample multiple CoT paths and take majority vote |
| Solving Quantitative Reasoning Problems with Language Models (Minerva) | [arXiv:2206.14858](https://arxiv.org/abs/2206.14858) | Math reasoning with LLMs |
| DeepSeek-R1: Incentivizing Reasoning Capability in LLMs via Reinforcement Learning | [arXiv:2501.12948](https://arxiv.org/abs/2501.12948) | RL-trained reasoning model rivaling OpenAI o1 |
| Scaling LLM Test-Time Compute Optimally can be More Effective than Scaling Model Parameters | [arXiv:2408.03314](https://arxiv.org/abs/2408.03314) | Foundational paper behind test-time compute scaling (thinking tokens) |
| s1: Simple Test-Time Scaling | [arXiv:2501.19393](https://arxiv.org/abs/2501.19393) | Budget forcing for efficient test-time compute |
| Let's Verify Step by Step | [arXiv:2305.20050](https://arxiv.org/abs/2305.20050) | Process Reward Models (PRM) for step-by-step verification |

## Reinforcement Learning from Human Feedback (RLHF) and Alignment

| Title | Link | Notes |
|-------|------|-------|
| Training Language Models to Follow Instructions with Human Feedback (InstructGPT) | [arXiv:2203.02155](https://arxiv.org/abs/2203.02155) | The foundational RLHF paper from OpenAI |
| Direct Preference Optimization: Your Language Model is Secretly a Reward Model (DPO) | [arXiv:2305.18290](https://arxiv.org/abs/2305.18290) | Simplified RLHF — no reward model needed |
| ORPO: Monolithic Preference Optimization without Reference Model | [arXiv:2403.07691](https://arxiv.org/abs/2403.07691) | Even simpler preference optimization |
| Constitutional AI: Harmlessness from AI Feedback (CAI) | [arXiv:2212.08073](https://arxiv.org/abs/2212.08073) | Anthropic's self-improvement alignment approach |
| Group Relative Policy Optimization (GRPO) | [arXiv:2402.03300](https://arxiv.org/abs/2402.03300) | DeepSeek's RL method — no critic model needed |

## Retrieval-Augmented Generation (RAG)

| Title | Link | Notes |
|-------|------|-------|
| Retrieval-Augmented Generation for Knowledge-Intensive NLP Tasks | [arXiv:2005.11401](https://arxiv.org/abs/2005.11401) | The original RAG paper by Meta |
| ColBERT: Efficient and Effective Passage Search via Contextualized Late Interaction | [arXiv:2004.12832](https://arxiv.org/abs/2004.12832) | Late interaction retrieval — fast and accurate |
| Self-RAG: Learning to Retrieve, Generate, and Critique through Self-Reflection | [arXiv:2310.11511](https://arxiv.org/abs/2310.11511) | LLM decides when and what to retrieve |
| Corrective RAG (CRAG) | [arXiv:2401.15884](https://arxiv.org/abs/2401.15884) | Evaluates retrieval quality and self-corrects |
| RAPTOR: Recursive Abstractive Processing for Tree-Organized Retrieval | [arXiv:2401.18059](https://arxiv.org/abs/2401.18059) | Hierarchical summarization for multi-level retrieval |
| Adaptive-RAG: Learning to Adapt Retrieval-Augmented Large Language Models through Question Complexity | [arXiv:2403.14403](https://arxiv.org/abs/2403.14403) | Routes queries to different retrieval strategies based on complexity |
| GraphRAG: From Local to Global | [arXiv:2404.16130](https://arxiv.org/abs/2404.16130) | Microsoft's knowledge graph approach to RAG |

## AI Agents and Tool Use

| Title | Link | Notes |
|-------|------|-------|
| ReAct: Synergizing Reasoning and Acting in Language Models | [arXiv:2210.03629](https://arxiv.org/abs/2210.03629) | Interleaving reasoning traces with actions |
| Toolformer: Language Models Can Teach Themselves to Use Tools | [arXiv:2302.04761](https://arxiv.org/abs/2302.04761) | Self-supervised tool-use learning |
| Voyager: An Open-Ended Embodied Agent with Large Language Models | [arXiv:2305.16291](https://arxiv.org/abs/2305.16291) | Autonomous exploration agent in Minecraft |
| AutoGen: Enabling Next-Gen LLM Applications via Multi-Agent Conversation | [arXiv:2308.08155](https://arxiv.org/abs/2308.08155) | Microsoft's multi-agent conversation framework |
| SWE-Agent: Agent-Computer Interfaces Enable Automated Software Engineering | [arXiv:2405.15793](https://arxiv.org/abs/2405.15793) | Agents that autonomously resolve GitHub issues |
| OpenHands: An Open Platform for AI Software Developers as Generalist Agents | [arXiv:2407.16741](https://arxiv.org/abs/2407.16741) | Open-source agentic coding platform |

## Fine-Tuning and Adaptation

| Title | Link | Notes |
|-------|------|-------|
| LoRA: Low-Rank Adaptation of Large Language Models | [arXiv:2106.09685](https://arxiv.org/abs/2106.09685) | Parameter-efficient fine-tuning — now ubiquitous |
| QLoRA: Efficient Finetuning of Quantized Language Models | [arXiv:2305.14314](https://arxiv.org/abs/2305.14314) | Fine-tune 65B models on a single 48GB GPU |
| Instruction Tuning for Large Language Models: A Survey | [arXiv:2308.10792](https://arxiv.org/abs/2308.10792) | Comprehensive survey on instruction tuning |
| DoRA: Weight-Decomposed Low-Rank Adaptation | [arXiv:2402.09353](https://arxiv.org/abs/2402.09353) | Improves on LoRA by decomposing weight magnitude and direction |
| Scaling Data-Constrained Language Models | [arXiv:2305.16264](https://arxiv.org/abs/2305.16264) | What to do when you run out of unique training data |

## Mixture of Experts (MoE)

| Title | Link | Notes |
|-------|------|-------|
| Mixtral of Experts | [arXiv:2401.04088](https://arxiv.org/abs/2401.04088) | Mistral's 8x7B sparse MoE — matches LLaMA 2 70B at 6x inference speed |
| Switch Transformers: Scaling to Trillion Parameter Models with Simple and Efficient Sparsity | [arXiv:2101.03961](https://arxiv.org/abs/2101.03961) | Google's foundational MoE for Transformers |
| DeepSeek-MoE: Towards Ultimate Expert Specialization in MoE Language Model | [arXiv:2401.06066](https://arxiv.org/abs/2401.06066) | Fine-grained expert segmentation and shared expert isolation |
| OLMoE: Open Mixture-of-Experts Language Models | [arXiv:2409.02060](https://arxiv.org/abs/2409.02060) | Fully open MoE model with 7B total / 1B active parameters |

## Long Context and Memory

| Title | Link | Notes |
|-------|------|-------|
| Extending Context Window of Large Language Models via Positional Interpolation | [arXiv:2306.15595](https://arxiv.org/abs/2306.15595) | Extend context length by interpolating RoPE positions |
| YaRN: Efficient Context Window Extension of Large Language Models | [arXiv:2309.00071](https://arxiv.org/abs/2309.00071) | Improved RoPE scaling for long contexts |
| MemGPT: Towards LLMs as Operating Systems | [arXiv:2310.08560](https://arxiv.org/abs/2310.08560) | Virtual memory management for unbounded context |
| Leave No Context Behind: Efficient Infinite Context Transformers with Infini-attention | [arXiv:2404.07143](https://arxiv.org/abs/2404.07143) | Google's approach to infinite context with compressive memory |

## Quantization and Compression

| Title | Link | Notes |
|-------|------|-------|
| GPTQ: Accurate Post-Training Quantization for Generative Pre-trained Transformers | [arXiv:2210.17323](https://arxiv.org/abs/2210.17323) | 3-4 bit quantization with minimal accuracy loss |
| AWQ: Activation-aware Weight Quantization for LLM Compression and Acceleration | [arXiv:2306.00978](https://arxiv.org/abs/2306.00978) | Protects salient weights during quantization |
| The Era of 1-bit LLMs: All Large Language Models are in 1.58 Bits (BitNet) | [arXiv:2402.17764](https://arxiv.org/abs/2402.17764) | Ternary {-1, 0, 1} weights matching full-precision performance |
| SqueezeLLM: Dense-and-Sparse Quantization | [arXiv:2306.07629](https://arxiv.org/abs/2306.07629) | Non-uniform quantization preserving outlier sensitivity |

## Inference Optimization and Serving

| Title | Link | Notes |
|-------|------|-------|
| Efficient Memory Management for LLM Serving with PagedAttention (vLLM) | [arXiv:2309.06180](https://arxiv.org/abs/2309.06180) | OS-style paged memory for KV cache — 24x throughput |
| Speculative Decoding | [arXiv:2211.17192](https://arxiv.org/abs/2211.17192) | Draft-then-verify for faster autoregressive generation |
| Medusa: Simple LLM Inference Acceleration Framework with Multiple Decoding Heads | [arXiv:2401.10774](https://arxiv.org/abs/2401.10774) | Parallel token prediction via additional decoding heads |
| SGLang: Efficient Execution of Structured Language Model Programs | [arXiv:2312.07104](https://arxiv.org/abs/2312.07104) | RadixAttention and structured generation for fast inference |
| Distilling the Knowledge in a Neural Network | [arXiv:1503.02531](https://arxiv.org/abs/1503.02531) | Hinton's foundational knowledge distillation paper |

## Multimodal Models

| Title | Link | Notes |
|-------|------|-------|
| LLaVA: Visual Instruction Tuning | [arXiv:2304.08485](https://arxiv.org/abs/2304.08485) | Connecting vision encoder to LLM for visual reasoning |
| LLaVA-1.5: Improved Baselines with Visual Instruction Tuning | [arXiv:2310.03744](https://arxiv.org/abs/2310.03744) | Simplified and improved multimodal architecture |
| Qwen2-VL: Enhancing Vision-Language Model's Perception of the World at Any Resolution | [arXiv:2409.12191](https://arxiv.org/abs/2409.12191) | Dynamic resolution for vision-language understanding |
| InternVL: Scaling up Vision Foundation Models and Aligning for Generic Visual-Linguistic Tasks | [arXiv:2312.14238](https://arxiv.org/abs/2312.14238) | Open-source GPT-4V alternative |
| Whisper: Robust Speech Recognition via Large-Scale Weak Supervision | [arXiv:2212.04356](https://arxiv.org/abs/2212.04356) | OpenAI's speech-to-text model trained on 680K hours |

## Code Generation

| Title | Link | Notes |
|-------|------|-------|
| Evaluating Large Language Models Trained on Code (Codex) | [arXiv:2107.03374](https://arxiv.org/abs/2107.03374) | OpenAI's code model powering GitHub Copilot |
| StarCoder 2 and The Stack v2: The Next Generation | [arXiv:2402.19173](https://arxiv.org/abs/2402.19173) | Open-source code LLM trained on permissively licensed data |
| SWE-bench: Can Language Models Resolve Real-World GitHub Issues? | [arXiv:2310.06770](https://arxiv.org/abs/2310.06770) | The definitive benchmark for agentic coding |
| Qwen2.5-Coder Technical Report | [arXiv:2409.12186](https://arxiv.org/abs/2409.12186) | Strong open-source code model family |

## Evaluation and Benchmarks

| Title | Link | Notes |
|-------|------|-------|
| Chatbot Arena: An Open Platform for Evaluating LLMs by Human Preference | [arXiv:2403.04132](https://arxiv.org/abs/2403.04132) | Crowdsourced blind evaluation with ELO rankings |
| MMLU: Measuring Massive Multitask Language Understanding | [arXiv:2009.03300](https://arxiv.org/abs/2009.03300) | Standard benchmark across 57 subjects |
| MMLU-Pro: A More Robust and Challenging Multi-Task Language Understanding Benchmark | [arXiv:2406.01574](https://arxiv.org/abs/2406.01574) | Harder successor to MMLU with 10 answer choices |
| GPQA: A Graduate-Level Google-Proof Q&A Benchmark | [arXiv:2311.12022](https://arxiv.org/abs/2311.12022) | Expert-level questions that domain PhDs struggle with |
| LiveBench: A Challenging, Contamination-Free LLM Benchmark | [arXiv:2406.19314](https://arxiv.org/abs/2406.19314) | Continuously updated to prevent data contamination |

## Surveys

| Title | Link | Notes |
|-------|------|-------|
| Large Language Models: A Survey | [arXiv:2402.06196](https://arxiv.org/abs/2402.06196) | Comprehensive overview of the LLM landscape |
| A Survey of Large Language Models | [arXiv:2303.18223](https://arxiv.org/abs/2303.18223) | Renmin University's widely cited LLM survey |
| Retrieval-Augmented Generation for Large Language Models: A Survey | [arXiv:2312.10997](https://arxiv.org/abs/2312.10997) | Comprehensive RAG survey covering paradigms and methods |
| A Survey on Mixture of Experts | [arXiv:2407.06204](https://arxiv.org/abs/2407.06204) | Covers MoE architectures from Switch Transformers to DeepSeek |
| The Landscape of Emerging AI Agent Architectures for Reasoning, Planning, and Tool Calling | [arXiv:2404.11584](https://arxiv.org/abs/2404.11584) | Survey on agent design patterns |

## Diffusion and Image Generation

| Title | Link | Notes |
|-------|------|-------|
| Denoising Diffusion Probabilistic Models | [arXiv:2006.11239](https://arxiv.org/abs/2006.11239) | The foundational diffusion model paper |
| High-Resolution Image Synthesis with Latent Diffusion Models (Stable Diffusion) | [arXiv:2112.10752](https://arxiv.org/abs/2112.10752) | Latent space diffusion enabling practical image generation |
| Flux | [Black Forest Labs](https://blackforestlabs.ai/) | State-of-the-art open image generation model |
| Scaling Rectified Flow Transformers for High-Resolution Image Synthesis (SD3) | [arXiv:2403.03206](https://arxiv.org/abs/2403.03206) | Rectified flow + DiT architecture for Stable Diffusion 3 |

---

*This list is actively maintained. Last updated: April 2026.*

*If you found this collection useful, please consider giving the repo a star.*
