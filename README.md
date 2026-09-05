# Awesome-LLM with stars

![](resources/image8.gif)

🔥 Large Language Models(LLM) have taken the ~~NLP community~~ ~~AI community~~ **the Whole World** by storm. Here is a curated list of papers about large language models, especially relating to ChatGPT. It also contains frameworks for LLM training, tools to deploy LLM, courses and tutorials about LLM and all publicly available LLM checkpoints and APIs.

## Trending LLM Projects

* [DeepSeek-V3](https://github.com/deepseek-ai/DeepSeek-V3) ⭐ 104,435 | 🐛 217 | 🌐 Python | 📅 2025-08-28 - First open-sourced GPT-4o level model.
* [DeepSeek-R1](https://github.com/deepseek-ai/DeepSeek-R1) ⭐ 92,022 | 🐛 33 | 📅 2025-06-27 - First-generation reasoning models from DeepSeek.
* [open-r1](https://github.com/huggingface/open-r1) ⭐ 26,450 | 🐛 340 | 🌐 Python | 📅 2026-04-02 - Fully open reproduction of DeepSeek-R1
* [TinyZero](https://github.com/Jiayi-Pan/TinyZero) ⭐ 13,229 | 🐛 82 | 🌐 Python | 📅 2026-02-27 - Clean, minimal, accessible reproduction of DeepSeek R1-Zero
* [Kimi-K2](https://github.com/MoonshotAI/Kimi-K2) ⭐ 11,108 | 🐛 71 | 📅 2026-01-21 - MoE language model with 32B active and 1T total parameters.
* [Qwen2.5-Max](https://qwenlm.github.io/blog/qwen2.5-max/) - Exploring the Intelligence of Large-scale MoE Model.
* [OpenAI o3-mini](https://openai.com/index/openai-o3-mini/) - Pushing the frontier of cost-effective reasoning.

## Table of Content

* [Awesome-LLM ](#awesome-llm-)
  * [Milestone Papers](#milestone-papers)
  * [Other Papers](#other-papers)
  * [LLM Leaderboard](#llm-leaderboard)
  * [Open LLM](#open-llm)
  * [LLM Data](#llm-data)
  * [LLM Evaluation](#llm-evaluation)
  * [LLM Training Framework](#llm-training-frameworks)
  * [LLM Inference](#llm-inference)
  * [LLM Applications](#llm-applications)
  * [LLM Tutorials and Courses](#llm-tutorials-and-courses)
  * [LLM Books](#llm-books)
  * [Great thoughts about LLM](#great-thoughts-about-llm)
  * [Miscellaneous](#miscellaneous)

## Milestone Papers

<details>

<summary> milestone papers </summary>

|   Date  |       keywords       |       Institute       | Paper                                                                                                                                                                                                              |
| :-----: | :------------------: | :-------------------: | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| 2017-06 |     Transformers     |         Google        | [Attention Is All You Need](https://arxiv.org/pdf/1706.03762.pdf)                                                                                                                                                  |
| 2018-06 |        GPT 1.0       |         OpenAI        | [Improving Language Understanding by Generative Pre-Training](https://www.cs.ubc.ca/~amuham01/LING530/papers/radford2018improving.pdf)                                                                             |
| 2018-10 |         BERT         |         Google        | [BERT: Pre-training of Deep Bidirectional Transformers for Language Understanding](https://aclanthology.org/N19-1423.pdf)                                                                                          |
| 2019-02 |        GPT 2.0       |         OpenAI        | [Language Models are Unsupervised Multitask Learners](https://d4mucfpksywv.cloudfront.net/better-language-models/language_models_are_unsupervised_multitask_learners.pdf)                                          |
| 2019-09 |      Megatron-LM     |         NVIDIA        | [Megatron-LM: Training Multi-Billion Parameter Language Models Using Model Parallelism](https://arxiv.org/pdf/1909.08053.pdf)                                                                                      |
| 2019-10 |          T5          |         Google        | [Exploring the Limits of Transfer Learning with a Unified Text-to-Text Transformer](https://jmlr.org/papers/v21/20-074.html)                                                                                       |
| 2019-10 |         ZeRO         |       Microsoft       | [ZeRO: Memory Optimizations Toward Training Trillion Parameter Models](https://arxiv.org/pdf/1910.02054.pdf)                                                                                                       |
| 2020-01 |      Scaling Law     |         OpenAI        | [Scaling Laws for Neural Language Models](https://arxiv.org/pdf/2001.08361.pdf)                                                                                                                                    |
| 2020-05 |        GPT 3.0       |         OpenAI        | [Language models are few-shot learners](https://papers.nips.cc/paper/2020/file/1457c0d6bfcb4967418bfb8ac142f64a-Paper.pdf)                                                                                         |
| 2021-01 |  Switch Transformers |         Google        | [Switch Transformers: Scaling to Trillion Parameter Models with Simple and Efficient Sparsity](https://arxiv.org/pdf/2101.03961.pdf)                                                                               |
| 2021-08 |         Codex        |         OpenAI        | [Evaluating Large Language Models Trained on Code](https://arxiv.org/pdf/2107.03374.pdf)                                                                                                                           |
| 2021-08 |   Foundation Models  |        Stanford       | [On the Opportunities and Risks of Foundation Models](https://arxiv.org/pdf/2108.07258.pdf)                                                                                                                        |
| 2021-09 |         FLAN         |         Google        | [Finetuned Language Models are Zero-Shot Learners](https://openreview.net/forum?id=gEZrGCozdqR)                                                                                                                    |
| 2021-10 |          T0          |   HuggingFace et al.  | [Multitask Prompted Training Enables Zero-Shot Task Generalization](https://arxiv.org/abs/2110.08207)                                                                                                              |
| 2021-12 |         GLaM         |         Google        | [GLaM: Efficient Scaling of Language Models with Mixture-of-Experts](https://arxiv.org/pdf/2112.06905.pdf)                                                                                                         |
| 2021-12 |        WebGPT        |         OpenAI        | [WebGPT: Browser-assisted question-answering with human feedback](https://www.semanticscholar.org/paper/WebGPT%3A-Browser-assisted-question-answering-with-Nakano-Hilton/2f3efe44083af91cef562c1a3451eee2f8601d22) |
| 2021-12 |         Retro        |        DeepMind       | [Improving language models by retrieving from trillions of tokens](https://www.deepmind.com/publications/improving-language-models-by-retrieving-from-trillions-of-tokens)                                         |
| 2021-12 |        Gopher        |        DeepMind       | [Scaling Language Models: Methods, Analysis & Insights from Training Gopher](https://arxiv.org/pdf/2112.11446.pdf)                                                                                                 |
| 2022-01 |          COT         |         Google        | [Chain-of-Thought Prompting Elicits Reasoning in Large Language Models](https://arxiv.org/pdf/2201.11903.pdf)                                                                                                      |
| 2022-01 |         LaMDA        |         Google        | [LaMDA: Language Models for Dialog Applications](https://arxiv.org/pdf/2201.08239.pdf)                                                                                                                             |
| 2022-01 |        Minerva       |         Google        | [Solving Quantitative Reasoning Problems with Language Models](https://arxiv.org/abs/2206.14858)                                                                                                                   |
| 2022-01 |  Megatron-Turing NLG |   Microsoft\&NVIDIA   | [Using Deep and Megatron to Train Megatron-Turing NLG 530B, A Large-Scale Generative Language Model](https://arxiv.org/pdf/2201.11990.pdf)                                                                         |
| 2022-03 |      InstructGPT     |         OpenAI        | [Training language models to follow instructions with human feedback](https://arxiv.org/pdf/2203.02155.pdf)                                                                                                        |
| 2022-04 |         PaLM         |         Google        | [PaLM: Scaling Language Modeling with Pathways](https://arxiv.org/pdf/2204.02311.pdf)                                                                                                                              |
| 2022-04 |      Chinchilla      |        DeepMind       | [Training Compute-Optimal Large Language Models](https://arxiv.org/pdf/2203.15556)                                                                                                                                 |
| 2022-05 |          OPT         |          Meta         | [OPT: Open Pre-trained Transformer Language Models](https://arxiv.org/pdf/2205.01068.pdf)                                                                                                                          |
| 2022-05 |          UL2         |         Google        | [Unifying Language Learning Paradigms](https://arxiv.org/abs/2205.05131v1)                                                                                                                                         |
| 2022-06 |  Emergent Abilities  |         Google        | [Emergent Abilities of Large Language Models](https://openreview.net/pdf?id=yzkSU5zdwD)                                                                                                                            |
| 2022-06 |       BIG-bench      |         Google        | [Beyond the Imitation Game: Quantifying and extrapolating the capabilities of language models](https://github.com/google/BIG-bench) ⚠️ Archived                                                                    |
| 2022-06 |        METALM        |       Microsoft       | [Language Models are General-Purpose Interfaces](https://arxiv.org/pdf/2206.06336.pdf)                                                                                                                             |
| 2022-09 |        Sparrow       |        DeepMind       | [Improving alignment of dialogue agents via targeted human judgements](https://arxiv.org/pdf/2209.14375.pdf)                                                                                                       |
| 2022-10 |     Flan-T5/PaLM     |         Google        | [Scaling Instruction-Finetuned Language Models](https://arxiv.org/pdf/2210.11416.pdf)                                                                                                                              |
| 2022-10 |       GLM-130B       |        Tsinghua       | [GLM-130B: An Open Bilingual Pre-trained Model](https://arxiv.org/pdf/2210.02414.pdf)                                                                                                                              |
| 2022-11 |         HELM         |        Stanford       | [Holistic Evaluation of Language Models](https://arxiv.org/pdf/2211.09110.pdf)                                                                                                                                     |
| 2022-11 |         BLOOM        |       BigScience      | [BLOOM: A 176B-Parameter Open-Access Multilingual Language Model](https://arxiv.org/pdf/2211.05100.pdf)                                                                                                            |
| 2022-11 |       Galactica      |          Meta         | [Galactica: A Large Language Model for Science](https://arxiv.org/pdf/2211.09085.pdf)                                                                                                                              |
| 2022-12 |        OPT-IML       |          Meta         | [OPT-IML: Scaling Language Model Instruction Meta Learning through the Lens of Generalization](https://arxiv.org/pdf/2212.12017)                                                                                   |
| 2023-01 | Flan 2022 Collection |         Google        | [The Flan Collection: Designing Data and Methods for Effective Instruction Tuning](https://arxiv.org/pdf/2301.13688.pdf)                                                                                           |
| 2023-02 |         LLaMA        |          Meta         | [LLaMA: Open and Efficient Foundation Language Models](https://research.facebook.com/publications/llama-open-and-efficient-foundation-language-models/)                                                            |
| 2023-02 |       Kosmos-1       |       Microsoft       | [Language Is Not All You Need: Aligning Perception with Language Models](https://arxiv.org/abs/2302.14045)                                                                                                         |
| 2023-03 |          LRU         |        DeepMind       | [Resurrecting Recurrent Neural Networks for Long Sequences](https://arxiv.org/abs/2303.06349)                                                                                                                      |
| 2023-03 |        PaLM-E        |         Google        | [PaLM-E: An Embodied Multimodal Language Model](https://palm-e.github.io)                                                                                                                                          |
| 2023-03 |         GPT 4        |         OpenAI        | [GPT-4 Technical Report](https://openai.com/research/gpt-4)                                                                                                                                                        |
| 2023-04 |         LLaVA        | UW–Madison\&Microsoft | [Visual Instruction Tuning](https://arxiv.org/abs/2304.08485)                                                                                                                                                      |
| 2023-04 |        Pythia        |   EleutherAI et al.   | [Pythia: A Suite for Analyzing Large Language Models Across Training and Scaling](https://arxiv.org/abs/2304.01373)                                                                                                |
| 2023-05 |       Dromedary      |       CMU et al.      | [Principle-Driven Self-Alignment of Language Models from Scratch with Minimal Human Supervision](https://arxiv.org/abs/2305.03047)                                                                                 |
| 2023-05 |        PaLM 2        |         Google        | [PaLM 2 Technical Report](https://ai.google/static/documents/palm2techreport.pdf)                                                                                                                                  |
| 2023-05 |         RWKV         |        Bo Peng        | [RWKV: Reinventing RNNs for the Transformer Era](https://arxiv.org/abs/2305.13048)                                                                                                                                 |
| 2023-05 |          DPO         |        Stanford       | [Direct Preference Optimization: Your Language Model is Secretly a Reward Model](https://arxiv.org/pdf/2305.18290.pdf)                                                                                             |
| 2023-05 |          ToT         |   Google\&Princeton   | [Tree of Thoughts: Deliberate Problem Solving with Large Language Models](https://arxiv.org/pdf/2305.10601.pdf)                                                                                                    |
| 2023-07 |        LLaMA2        |          Meta         | [Llama 2: Open Foundation and Fine-Tuned Chat Models](https://arxiv.org/pdf/2307.09288.pdf)                                                                                                                        |
| 2023-10 |      Mistral 7B      |        Mistral        | [Mistral 7B](https://arxiv.org/pdf/2310.06825.pdf)                                                                                                                                                                 |
| 2023-12 |         Mamba        |     CMU\&Princeton    | [Mamba: Linear-Time Sequence Modeling with Selective State Spaces](https://arxiv.org/pdf/2312.00752)                                                                                                               |
| 2024-01 |      DeepSeek-v2     |        DeepSeek       | [DeepSeek-V2: A Strong, Economical, and Efficient Mixture-of-Experts Language Model](https://arxiv.org/abs/2405.04434)                                                                                             |
| 2024-02 |         OLMo         |          Ai2          | [OLMo: Accelerating the Science of Language Models](https://arxiv.org/abs/2402.00838)                                                                                                                              |
| 2024-05 |        Mamba2        |     CMU\&Princeton    | [Transformers are SSMs: Generalized Models and Efficient Algorithms Through Structured State Space Duality](https://arxiv.org/abs/2405.21060)                                                                      |
| 2024-05 |        Llama3        |          Meta         | [The Llama 3 Herd of Models](https://arxiv.org/abs/2407.21783)                                                                                                                                                     |
| 2024-06 |        FineWeb       |      HuggingFace      | [The FineWeb Datasets: Decanting the Web for the Finest Text Data at Scale](https://arxiv.org/abs/2406.17557)                                                                                                      |
| 2024-09 |         OLMoE        |          Ai2          | [OLMoE: Open Mixture-of-Experts Language Models](https://arxiv.org/abs/2409.02060)                                                                                                                                 |
| 2024-12 |        Qwen2.5       |        Alibaba        | [Qwen2.5 Technical Report](https://arxiv.org/abs/2412.15115)                                                                                                                                                       |
| 2024-12 |      DeepSeek-V3     |        DeepSeek       | [DeepSeek-V3 Technical Report](https://arxiv.org/abs/2412.19437v1)                                                                                                                                                 |
| 2025-01 |      DeepSeek-R1     |        DeepSeek       | [DeepSeek-R1: Incentivizing Reasoning Capability in LLMs via Reinforcement Learning](https://arxiv.org/abs/2501.12948)                                                                                             |

</details>

## Other Papers

> \[!NOTE]
> If you're interested in the field of LLM, you may find the above list of milestone papers helpful to explore its history and state-of-the-art. However, each direction of LLM offers a unique set of insights and contributions, which are essential to understanding the field as a whole. For a detailed list of papers in various subfields, please refer to the following link:

<details>
  <summary> other papers </summary>

* [Awesome ChatGPT Prompts](https://github.com/f/awesome-chatgpt-prompts) ⭐ 169,389 | 🐛 74 | 🌐 HTML | 📅 2026-09-05 - A collection of prompt examples to be used with the ChatGPT model.

* [awesome-chatgpt-prompts-zh](https://github.com/PlexPt/awesome-chatgpt-prompts-zh) ⭐ 62,048 | 🐛 45 | 📅 2026-04-28 - A Chinese collection of prompt examples to be used with the ChatGPT model.

* [Awesome-Chinese-LLM](https://github.com/HqWu-HITCS/Awesome-Chinese-LLM) ⭐ 22,754 | 🐛 30 | 📅 2026-05-10 - 整理开源的中文大语言模型，以规模较小、可私有化部署、训练成本较低的模型为主，包括底座模型，垂直领域微调及应用，数据集与教程等。

* [LLMsPracticalGuide](https://github.com/Mooler0410/LLMsPracticalGuide) ⭐ 10,204 | 🐛 17 | 📅 2026-04-08 - A curated list of practical guide resources of LLMs

* [Awesome ChatGPT](https://github.com/humanloop/awesome-chatgpt) ⭐ 8,206 | 🐛 144 | 📅 2025-10-15 - Curated list of resources for ChatGPT and GPT-3 from OpenAI.

* [Awesome GPT-3](https://github.com/elyase/awesome-gpt3) ⚠️ Archived - a collection of demos and articles about the [OpenAI GPT-3 API](https://openai.com/blog/openai-api/).

* [Reasoning using Language Models](https://github.com/atfortes/LM-Reasoning-Papers) ⭐ 3,681 | 🐛 27 | 📅 2026-04-20 - Collection of papers and resources on Reasoning using Language Models.

* [LLMDatahub](https://github.com/Zjh-819/LLMDataHub) ⭐ 3,413 | 🐛 5 | 📅 2023-11-28 - a curated collection of datasets specifically designed for chatbot training, including links, size, language, usage, and a brief description of each dataset

* [Chain-of-Thought Hub](https://github.com/FranxYao/chain-of-thought-hub) ⭐ 2,774 | 🐛 27 | 🌐 Jupyter Notebook | 📅 2024-08-04 - Measuring LLMs' Reasoning Performance

* [Awesome-LLM-3D](https://github.com/ActiveVisionLab/Awesome-LLM-3D) ⭐ 2,254 | 🐛 7 | 📅 2026-04-16 - A curated list of Multi-modal Large Language Model in 3D world, including 3D understanding, reasoning, generation, and embodied agents.

* [Awesome-LLM-Systems](https://github.com/AmberLJC/LLMSys-PaperList) ⭐ 2,240 | 🐛 1 | 🌐 Python | 📅 2026-07-25 - Awesome LLM systems research papers.

* [Chain-of-Thoughts Papers](https://github.com/Timothyxxx/Chain-of-ThoughtsPapers) ⚠️ Archived -  A trend starts from "Chain of Thought Prompting Elicits Reasoning in Large Language Models.

* [Awesome-LLM-Compression](https://github.com/HuangOwen/Awesome-LLM-Compression) ⭐ 1,866 | 🐛 2 | 📅 2026-08-27 - Awesome LLM compression research papers and tools.

* [Awesome LLM Security](https://github.com/corca-ai/awesome-llm-security) ⭐ 1,692 | 🐛 206 | 📅 2025-08-20 - A curation of awesome tools, documents and projects about LLM Security.

* [awesome-japanese-llm](https://github.com/llm-jp/awesome-japanese-llm) ⭐ 1,425 | 🐛 0 | 🌐 TypeScript | 📅 2026-09-01 - 日本語LLMまとめ - Overview of Japanese LLMs.

* [Awesome-Code-LLM](https://github.com/huybery/Awesome-Code-LLM) ⭐ 1,290 | 🐛 5 | 📅 2024-12-10 - An awesome and curated list of best code-LLM for research.

* [ModelEditingPapers](https://github.com/zjunlp/ModelEditingPapers) ⭐ 1,247 | 🐛 0 | 📅 2026-08-20 - A paper & resource list on model editing for large language models.

* [awesome-hallucination-detection](https://github.com/EdinburghNLP/awesome-hallucination-detection) ⭐ 1,127 | 🐛 0 | 📅 2026-07-24 - List of papers on hallucination detection in LLMs.

* [Awesome GPT](https://github.com/formulahendry/awesome-gpt) ⭐ 1,044 | 🐛 29 | 📅 2024-05-29 - A curated list of awesome projects and resources related to GPT, ChatGPT, OpenAI, LLM, and more.

* [Instruction-Tuning-Papers](https://github.com/SinclairCoder/Instruction-Tuning-Papers) ⭐ 767 | 🐛 0 | 📅 2023-07-20 - A trend starts from `Natrural-Instruction` (ACL 2022), `FLAN` (ICLR 2022) and `T0` (ICLR 2022).

* [Awesome-Align-LLM-Human](https://github.com/GaryYufei/AlignLLMHumanSurvey) ⭐ 738 | 🐛 0 | 📅 2023-09-11 - A collection of papers and resources about aligning large language models (LLMs) with human.

* [awesome-llm-webapps](https://github.com/snowfort-ai/awesome-llm-webapps) ⭐ 718 | 🐛 13 | 📅 2025-06-29 - A collection of open source, actively maintained web apps for LLM applications.

* [LLM4Opt](https://github.com/FeiLiu36/LLM4Opt) ⭐ 398 | 🐛 0 | 📅 2026-03-31 - Applying Large language models (LLMs) for diverse optimization tasks (Opt) is an emerging research area. This is a collection of references and papers of LLM4Opt.

* [Awesome LLM Human Preference Datasets](https://github.com/PolisAI/awesome-llm-human-preference-datasets) ⭐ 391 | 🐛 0 | 📅 2023-10-04 - a collection of human preference datasets for LLM instruction tuning, RLHF and evaluation.

* [Awesome-LLM-hallucination](https://github.com/LuckyyySTA/Awesome-LLM-hallucination) ⭐ 338 | 🐛 4 | 📅 2024-03-11 - LLM hallucination paper list.

* [Awesome-LLM-Healthcare](https://github.com/mingze-yuan/Awesome-LLM-Healthcare) ⭐ 270 | 🐛 0 | 📅 2023-12-23 - The paper list of the review on LLMs in medicine.

* [LLM Reading List](https://github.com/crazyofapple/Reading_groups/) ⭐ 203 | 🐛 0 | 📅 2023-08-08 - A paper & resource list of large language models.

* [Awesome Deliberative Prompting](https://github.com/logikon-ai/awesome-deliberative-prompting) ⚠️ Archived - How to ask LLMs to produce reliable reasoning and make reason-responsive decisions.

* [awesome-language-model-analysis](https://github.com/Furyton/awesome-language-model-analysis) ⭐ 102 | 🐛 11 | 🌐 Python | 📅 2026-07-29 - This paper list focuses on the theoretical or empirical analysis of language models, e.g., the learning dynamics, expressive capacity, interpretability, generalization, and other interesting topics.

* [RWKV-howto](https://github.com/Hannibal046/RWKV-howto) ⭐ 27 | 🐛 0 | 📅 2023-06-08 - possibly useful materials and tutorial for learning RWKV.

* [Awesome-LLM-Inference](https://github.com/DefTruth/Awesome-LLM-Inference) ⭐ 21 | 🐛 0 | 📅 2025-03-30 - A curated list of Awesome LLM Inference Paper with codes.

</details>

## LLM Leaderboard

* [Chatbot Arena Leaderboard](https://huggingface.co/spaces/lmsys/chatbot-arena-leaderboard) - a benchmark platform for large language models (LLMs) that features anonymous, randomized battles in a crowdsourced manner.
* [LiveBench](https://livebench.ai/#/) - A Challenging, Contamination-Free LLM Benchmark.
* [Open LLM Leaderboard](https://huggingface.co/spaces/open-llm-leaderboard/open_llm_leaderboard) - aims to track, rank, and evaluate LLMs and chatbots as they are released.
* [AlpacaEval](https://tatsu-lab.github.io/alpaca_eval/) - An Automatic Evaluator for Instruction-following Language Models using Nous benchmark suite.

<details>
  <summary> other leaderboards </summary>

* [Chinese Large Model Leaderboard](https://github.com/jeinlee1991/chinese-llm-benchmark) ⭐ 6,422 | 🐛 18 | 📅 2026-09-04 - an expert-driven benchmark for Chineses LLMs.
* [ACLUE](https://github.com/isen-zhang/ACLUE) ⭐ 35 | 🐛 0 | 🌐 Python | 📅 2024-03-20 - an evaluation benchmark focused on ancient Chinese language comprehension.
* [BeHonest](https://gair-nlp.github.io/BeHonest/#leaderboard) - A pioneering benchmark specifically designed to assess honesty in LLMs comprehensively.
* [Berkeley Function-Calling Leaderboard](https://gorilla.cs.berkeley.edu/leaderboard.html) - evaluates LLM's ability to call external functions/tools.
* [CompassRank](https://rank.opencompass.org.cn) - CompassRank is dedicated to exploring the most advanced language and visual models, offering a comprehensive, objective, and neutral evaluation reference for the industry and research.
* [CompMix](https://qa.mpi-inf.mpg.de/compmix) - a benchmark evaluating QA methods that operate over a mixture of heterogeneous input sources (KB, text, tables, infoboxes).
* [DreamBench++](https://dreambenchplus.github.io/#leaderboard) - a benchmark for evaluating the performance of large language models (LLMs) in various tasks related to both textual and visual imagination.
* [FELM](https://hkust-nlp.github.io/felm) - a meta-benchmark that evaluates how well factuality evaluators assess the outputs of large language models (LLMs).
* [InfiBench](https://infi-coder.github.io/infibench) - a benchmark designed to evaluate large language models (LLMs) specifically in their ability to answer real-world coding-related questions.
* [LawBench](https://lawbench.opencompass.org.cn/leaderboard) - a benchmark designed to evaluate large language models in the legal domain.
* [LLMEval](http://llmeval.com) - focuses on understanding how these models perform in various scenarios and analyzing results from an interpretability perspective.
* [M3CoT](https://lightchen233.github.io/m3cot.github.io/leaderboard.html) - a benchmark that evaluates large language models on a variety of multimodal reasoning tasks, including language, natural and social sciences, physical and social commonsense, temporal reasoning, algebra, and geometry.
* [MathEval](https://matheval.ai) - a comprehensive benchmarking platform designed to evaluate large models' mathematical abilities across 20 fields and nearly 30,000 math problems.
* [MixEval](https://mixeval.github.io/#leaderboard) - a ground-truth-based dynamic benchmark derived from off-the-shelf benchmark mixtures, which evaluates LLMs with a highly capable model ranking (i.e., 0.96 correlation with Chatbot Arena) while running locally and quickly (6% the time and cost of running MMLU).
* [MMedBench](https://henrychur.github.io/MultilingualMedQA) - a benchmark that evaluates large language models' ability to answer medical questions across multiple languages.
* [MMToM-QA](https://chuanyangjin.com/mmtom-qa-leaderboard) - a multimodal question-answering benchmark designed to evaluate AI models' cognitive ability to understand human beliefs and goals.
* [OlympicArena](https://gair-nlp.github.io/OlympicArena/#leaderboard) - a benchmark for evaluating AI models across multiple academic disciplines like math, physics, chemistry, biology, and more.
* [PubMedQA](https://pubmedqa.github.io) - a biomedical question-answering benchmark designed for answering research-related questions using PubMed abstracts.
* [SciBench](https://scibench-ucla.github.io/#leaderboard) -  benchmark designed to evaluate large language models (LLMs) on solving complex, college-level scientific problems from domains like chemistry, physics, and mathematics.
* [SuperBench](https://fm.ai.tsinghua.edu.cn/superbench/#/leaderboard) - a benchmark platform designed for evaluating large language models (LLMs) on a range of tasks, particularly focusing on their performance in different aspects such as natural language understanding, reasoning, and generalization.
* [SuperLim](https://lab.kb.se/leaderboard/results) - a Swedish language understanding benchmark that evaluates natural language processing (NLP) models on various tasks such as argumentation analysis, semantic similarity, and textual entailment.
* [TAT-DQA](https://nextplusplus.github.io/TAT-DQA) - a large-scale Document Visual Question Answering (VQA) dataset designed for complex document understanding, particularly in financial reports.
* [TAT-QA](https://nextplusplus.github.io/TAT-QA) - a large-scale question-answering benchmark focused on real-world financial data, integrating both tabular and textual information.
* [VisualWebArena](https://jykoh.com/vwa) - a benchmark designed to assess the performance of multimodal web agents on realistic visually grounded tasks.
* [We-Math](https://we-math.github.io/#leaderboard) - a benchmark that evaluates large multimodal models (LMMs) on their ability to perform human-like mathematical reasoning.
* [WHOOPS!](https://whoops-benchmark.github.io) - a benchmark dataset testing AI's ability to reason about visual commonsense through images that defy normal expectations.

</details>

## Open LLM

<details>
<summary>DeepSeek</summary>

* [DeepSeek-V3](https://github.com/deepseek-ai/DeepSeek-V3) ⭐ 104,435 | 🐛 217 | 🌐 Python | 📅 2025-08-28
* [DeepSeek-R1](https://github.com/deepseek-ai/DeepSeek-R1) ⭐ 92,022 | 🐛 33 | 📅 2025-06-27
* [DeepSeek-Coder-v2-16|236B-MOE](https://github.com/deepseek-ai/DeepSeek-Coder-V2) ⭐ 7,005 | 🐛 78 | 📅 2025-11-11
* [DeepSeek-Math-7B](https://huggingface.co/collections/deepseek-ai/deepseek-math-65f2962739da11599e441681)
* [DeepSeek-Coder-1.3|6.7|7|33B](https://huggingface.co/collections/deepseek-ai/deepseek-coder-65f295d7d8a0a29fe39b4ec4)
* [DeepSeek-VL-1.3|7B](https://huggingface.co/collections/deepseek-ai/deepseek-vl-65f295948133d9cf92b706d3)
* [DeepSeek-MoE-16B](https://huggingface.co/collections/deepseek-ai/deepseek-moe-65f29679f5cf26fe063686bf)
* [DeepSeek-v2-236B-MoE](https://arxiv.org/abs/2405.04434)
* [DeepSeek-V2.5](https://huggingface.co/deepseek-ai/DeepSeek-V2.5)

</details>
<details>
<summary>Alibaba</summary>

* [Qwen-1.8B|7B|14B|72B](https://huggingface.co/collections/Qwen/qwen-65c0e50c3f1ab89cb8704144)
* [Qwen1.5-0.5B|1.8B|4B|7B|14B|32B|72B|110B|MoE-A2.7B](https://qwenlm.github.io/blog/qwen1.5/)
* [Qwen2-0.5B|1.5B|7B|57B-A14B-MoE|72B](https://qwenlm.github.io/blog/qwen2)
* [Qwen2.5-0.5B|1.5B|3B|7B|14B|32B|72B](https://qwenlm.github.io/blog/qwen2.5/)
* [CodeQwen1.5-7B](https://qwenlm.github.io/blog/codeqwen1.5/)
* [Qwen2.5-Coder-1.5B|7B|32B](https://qwenlm.github.io/blog/qwen2.5-coder/)
* [Qwen2-Math-1.5B|7B|72B](https://qwenlm.github.io/blog/qwen2-math/)
* [Qwen2.5-Math-1.5B|7B|72B](https://qwenlm.github.io/blog/qwen2.5-math/)
* [Qwen-VL-7B](https://huggingface.co/Qwen/Qwen-VL)
* [Qwen2-VL-2B|7B|72B](https://qwenlm.github.io/blog/qwen2-vl/)
* [Qwen2-Audio-7B](https://qwenlm.github.io/blog/qwen2-audio/)
* [Qwen2.5-VL-3|7|72B](https://qwenlm.github.io/blog/qwen2.5-vl/)
* [Qwen2.5-1M-7|14B](https://qwenlm.github.io/blog/qwen2.5-1m/)

</details>

<details>
<summary>Meta</summary>

* [Llama 3.2-1|3|11|90B](https://llama.meta.com/)
* [Llama 3.1-8|70|405B](https://llama.meta.com/)
* [Llama 3-8|70B](https://llama.meta.com/llama3/)
* [Llama 2-7|13|70B](https://llama.meta.com/llama2/)
* [Llama 1-7|13|33|65B](https://ai.facebook.com/blog/large-language-model-llama-meta-ai/)
* [OPT-1.3|6.7|13|30|66B](https://arxiv.org/abs/2205.01068)

</details>

<details>
<summary>Mistral AI</summary>

* [Codestral-7|22B](https://mistral.ai/news/codestral/)
* [Mistral-7B](https://mistral.ai/news/announcing-mistral-7b/)
* [Mixtral-8x7B](https://mistral.ai/news/mixtral-of-experts/)
* [Mixtral-8x22B](https://mistral.ai/news/mixtral-8x22b/)

</details>
<details>
<summary>Google</summary>

* [RecurrentGemma-2B](https://github.com/google-deepmind/recurrentgemma) ⭐ 685 | 🐛 4 | 🌐 Python | 📅 2026-02-06
* [Gemma2-9|27B](https://blog.google/technology/developers/google-gemma-2/)
* [Gemma-2|7B](https://blog.google/technology/developers/gemma-open-models/)
* [T5](https://arxiv.org/abs/1910.10683)

</details>
<details>
<summary>Apple</summary>

* [OpenELM-1.1|3B](https://huggingface.co/apple/OpenELM)

</details>
<details>
<summary>Microsoft</summary>

* [Phi1-1.3B](https://huggingface.co/microsoft/phi-1)
* [Phi2-2.7B](https://huggingface.co/microsoft/phi-2)
* [Phi3-3.8|7|14B](https://huggingface.co/microsoft/Phi-3-mini-4k-instruct)

</details>
<details>
<summary>AllenAI</summary>

* [OLMo-7B](https://huggingface.co/collections/allenai/olmo-suite-65aeaae8fe5b6b2122b46778)

</details>
<details>
<summary>xAI</summary>

* [Grok-1-314B-MoE](https://x.ai/blog/grok-os)

</details>
<details>
<summary>Cohere</summary>

* [Command R-35B](https://huggingface.co/CohereForAI/c4ai-command-r-v01)

</details>

<details>
<summary>01-ai</summary>

* [Yi-34B](https://huggingface.co/collections/01-ai/yi-2023-11-663f3f19119ff712e176720f)
* [Yi1.5-6|9|34B](https://huggingface.co/collections/01-ai/yi-15-2024-05-663f3ecab5f815a3eaca7ca8)
* [Yi-VL-6B|34B](https://huggingface.co/collections/01-ai/yi-vl-663f557228538eae745769f3)

</details>

<details>
<summary>Baichuan</summary>

* [Baichuan-7|13B](https://huggingface.co/baichuan-inc)
* [Baichuan2-7|13B](https://huggingface.co/baichuan-inc)

</details>

<details>
<summary>Nvidia</summary>

* [Nemotron-4-340B](https://huggingface.co/nvidia/Nemotron-4-340B-Instruct)

</details>

<details>
<summary>BLOOM</summary>

* [BLOOMZ\&mT0](https://huggingface.co/bigscience/bloomz)

</details>
<details>
<summary>Zhipu AI</summary>

* [GLM-2|6|10|13|70B](https://huggingface.co/THUDM)
* [CogVLM2-19B](https://huggingface.co/collections/THUDM/cogvlm2-6645f36a29948b67dc4eef75)

</details>
<details>
<summary>OpenBMB</summary>

* [MiniCPM-2B](https://huggingface.co/collections/openbmb/minicpm-2b-65d48bf958302b9fd25b698f)
* [OmniLLM-12B](https://huggingface.co/openbmb/OmniLMM-12B)
* [VisCPM-10B](https://huggingface.co/openbmb/VisCPM-Chat)
* [CPM-Bee-1|2|5|10B](https://huggingface.co/collections/openbmb/cpm-bee-65d491cc84fc93350d789361)

</details>
<details>
<summary>RWKV Foundation</summary>

* [RWKV-v4|5|6](https://huggingface.co/RWKV)minicpm-2b-65d48bf958302b9fd25b698f)

</details>

<details>
<summary>ElutherAI</summary>

* [Pythia-1|1.4|2.8|6.9|12B](https://github.com/EleutherAI/pythia) ⭐ 2,920 | 🐛 26 | 🌐 Jupyter Notebook | 📅 2025-11-15

</details>

<details>
<summary>Stability AI</summary>

* [StableLM-3B](https://huggingface.co/stabilityai/stablelm-3b-4e1t)
* [StableLM-v2-1.6B](https://huggingface.co/stabilityai/stablelm-2-1_6b)
* [StableLM-v2-12B](https://huggingface.co/stabilityai/stablelm-2-12b)
* [StableCode-3B](https://huggingface.co/collections/stabilityai/stable-code-64f9dfb4ebc8a1be0a3f7650)

</details>
<details>
<summary>BigCode</summary>

* [StarCoder-1|3|7B](https://huggingface.co/collections/bigcode/%E2%AD%90-starcoder-64f9bd5740eb5daaeb81dbec)
* [StarCoder2-3|7|15B](https://huggingface.co/collections/bigcode/starcoder2-65de6da6e87db3383572be1a)

</details>
<details>
<summary>DataBricks</summary>

* [MPT-7B](https://www.databricks.com/blog/mpt-7b)
* [DBRX-132B-MoE](https://www.databricks.com/blog/introducing-dbrx-new-state-art-open-llm)

</details>
<details>
<summary>Shanghai AI Laboratory</summary>

* [InternLM2-1.8|7|20B](https://huggingface.co/collections/internlm/internlm2-65b0ce04970888799707893c)
* [InternLM-Math-7B|20B](https://huggingface.co/collections/internlm/internlm2-math-65b0ce88bf7d3327d0a5ad9f)
* [InternLM-XComposer2-1.8|7B](https://huggingface.co/collections/internlm/internlm-xcomposer2-65b3706bf5d76208998e7477)
* [InternVL-2|6|14|26](https://huggingface.co/collections/OpenGVLab/internvl-65b92d6be81c86166ca0dde4)

</details>
<details>
<summary>Moonshot AI</summary>

* [Moonlight-A3B](https://huggingface.co/collections/moonshotai/moonlight-a3b-67f67b029cecfdce34f4dc23)
* [Kimi-VL-A3B](https://huggingface.co/collections/moonshotai/kimi-vl-a3b-67f67b6ac91d3b03d382dd85)
* [Kimi-K2](https://huggingface.co/collections/moonshotai/kimi-k2-6871243b990f2af5ba60617d)

</details>

## LLM Data

> Reference: [LLMDataHub](https://github.com/Zjh-819/LLMDataHub) ⭐ 3,413 | 🐛 5 | 📅 2023-11-28

* [Datatrove](https://github.com/huggingface/datatrove) ⭐ 3,323 | 🐛 101 | 🌐 Python | 📅 2026-08-13 - Freeing data processing from scripting madness by providing a set of platform-agnostic customizable pipeline processing blocks.
* [IBM data-prep-kit](https://github.com/IBM/data-prep-kit) ⭐ 958 | 🐛 231 | 🌐 HTML | 📅 2026-09-03 - Open-Source Toolkit for Efficient Unstructured Data Processing with Pre-built Modules and Local to Cluster Scalability.
* [Dingo](https://github.com/DataEval/dingo) ⭐ 753 | 🐛 5 | 🌐 Python | 📅 2026-09-03 - Dingo: A Comprehensive Data Quality Evaluation Tool
* [FastDatasets](https://github.com/ZhuLinsen/FastDatasets) ⭐ 222 | 🐛 0 | 🌐 Python | 📅 2025-08-31 - A powerful tool for creating high-quality training datasets for Large Language Models

## LLM Evaluation:

* [lm-evaluation-harness](https://github.com/EleutherAI/lm-evaluation-harness) ⭐ 13,894 | 🐛 936 | 🌐 Python | 📅 2026-09-01 - A framework for few-shot evaluation of language models.
* [simple-evals](https://github.com/openai/simple-evals) ⭐ 4,625 | 🐛 62 | 🌐 Python | 📅 2026-04-22 - Eval tools by OpenAI.
* [lighteval](https://github.com/huggingface/lighteval) ⭐ 2,535 | 🐛 405 | 🌐 Python | 📅 2026-08-11 - a lightweight LLM evaluation suite that Hugging Face has been using internally.

<details>
<summary>other evaluation frameworks</summary>

* [Ragas](https://github.com/explodinggradients/ragas) ⭐ 15,628 | 🐛 594 | 🌐 Python | 📅 2026-02-24 - a framework that helps you evaluate your Retrieval Augmented Generation (RAG) pipelines.
* [Giskard](https://github.com/Giskard-AI/giskard) ⭐ 5,802 | 🐛 62 | 🌐 Python | 📅 2026-09-04 - Testing & evaluation library for LLM applications, in particular RAGs
* [HELM](https://github.com/stanford-crfm/helm) ⭐ 2,902 | 🐛 104 | 🌐 Python | 📅 2026-09-01 - Holistic Evaluation of Language Models (HELM), a framework to increase the transparency of language models.
* [instruct-eval](https://github.com/declare-lab/instruct-eval) ⭐ 552 | 🐛 24 | 🌐 Python | 📅 2024-03-10 - This repository contains code to quantitatively evaluate instruction-tuned models such as Alpaca and Flan-T5 on held-out tasks.
* [MixEval](https://github.com/Psycoy/MixEval) ⭐ 254 | 🐛 7 | 🌐 Python | 📅 2024-11-10 - A reliable click-and-go evaluation suite compatible with both open-source and proprietary models, supporting MixEval and other benchmarks.
* [OLMO-eval](https://github.com/allenai/OLMo-Eval) ⭐ 69 | 🐛 56 | 🌐 Python | 📅 2026-09-05 - a repository for evaluating open language models.
* [LangSmith](https://www.langchain.com/langsmith) - a unified platform from LangChain framework for: evaluation, collaboration HITL (Human In The Loop), logging and monitoring LLM applications.

</details>

## LLM Training Frameworks

* [DeepSpeed](https://github.com/microsoft/DeepSpeed) ⭐ 43,065 | 🐛 1,364 | 🌐 Python | 📅 2026-09-05 - DeepSpeed is a deep learning optimization library that makes distributed training and inference easy, efficient, and effective.
* [Megatron-LM](https://github.com/NVIDIA/Megatron-LM) ⭐ 17,751 | 🐛 1,252 | 🌐 Python | 📅 2026-09-05 - Ongoing research training transformer models at scale.
* [Litgpt](https://github.com/Lightning-AI/litgpt) ⭐ 13,651 | 🐛 289 | 🌐 Python | 📅 2026-09-04 - 20+ high-performance LLMs with recipes to pretrain, finetune and deploy at scale.
* [torchtitan](https://github.com/pytorch/torchtitan) ⭐ 5,704 | 🐛 706 | 🌐 Python | 📅 2026-09-05 - A native PyTorch Library for large model training.
* [Meta Lingua](https://github.com/facebookresearch/lingua) ⭐ 4,764 | 🐛 14 | 🌐 Python | 📅 2025-07-18 - a lean, efficient, and easy-to-hack codebase to research LLMs.
* [nanotron](https://github.com/huggingface/nanotron) ⭐ 2,808 | 🐛 151 | 🌐 Python | 📅 2026-05-26 - Minimalistic large language model 3D-parallelism training.

<details>
<summary>other frameworks</summary>

* [unslothai](https://github.com/unslothai/unsloth) ⭐ 75,665 | 🐛 1,436 | 🌐 Python | 📅 2026-09-05 - A framework that specializes in efficient fine-tuning. On its GitHub page, you can find ready-to-use fine-tuning templates for various LLMs, allowing you to easily train your own data for free on the Google Colab cloud.
* [Colossal-AI](https://github.com/hpcaitech/ColossalAI) ⭐ 41,444 | 🐛 505 | 🌐 Python | 📅 2026-08-31 - Making large AI models cheaper, faster, and more accessible.
* [veRL](https://github.com/volcengine/verl) ⭐ 23,306 | 🐛 1,240 | 🌐 Python | 📅 2026-09-04 - veRL is a flexible and efficient RL framework for LLMs.
* [NeMo Framework](https://github.com/NVIDIA/NeMo) ⭐ 18,390 | 🐛 301 | 🌐 Python | 📅 2026-09-05 - Generative AI framework built for researchers and PyTorch developers working on Large Language Models (LLMs), Multimodal Models (MMs), Automatic Speech Recognition (ASR), Text to Speech (TTS), and Computer Vision (CV) domains.
* [Axolotl](https://github.com/axolotl-ai-cloud/axolotl) ⭐ 12,441 | 🐛 250 | 🌐 Python | 📅 2026-09-04 - Open-source framework for fine-tuning and evaluating LLMs. It simplifies the process of experimenting with different training configurations and makes it easy to reproduce and share results, supporting features like LoRA, QLoRA, DeepSpeed, PEFT, and multi-GPU setups.
* [OpenRLHF](https://github.com/OpenRLHF/OpenRLHF) ⭐ 9,976 | 🐛 369 | 🌐 Python | 📅 2026-08-13 - An Easy-to-use, Scalable and High-performance RLHF Framework (70B+ PPO Full Tuning & Iterative DPO & LoRA & RingAttention & RFT).
* [GPT-NeoX](https://github.com/EleutherAI/gpt-neox) ⭐ 7,461 | 🐛 111 | 🌐 Python | 📅 2026-09-04 - An implementation of model parallel autoregressive transformers on GPUs, based on the DeepSpeed library.
* [torchtune](https://github.com/pytorch/torchtune) ⭐ 5,805 | 🐛 460 | 🌐 Python | 📅 2026-09-05 - A Native-PyTorch Library for LLM Fine-tuning.
* [Transformer Engine](https://github.com/NVIDIA/TransformerEngine) ⭐ 3,522 | 🐛 341 | 🌐 Python | 📅 2026-09-05 - A library for accelerating Transformer model training on NVIDIA GPUs.
* [ROLL](https://github.com/alibaba/ROLL) ⭐ 3,383 | 🐛 128 | 🌐 Python | 📅 2026-09-05 - An Efficient and User-Friendly Scaling Library for Reinforcement Learning with Large Language Models.
* [maxtext](https://github.com/AI-Hypercomputer/maxtext) ⭐ 2,412 | 🐛 338 | 🌐 Python | 📅 2026-09-05 - A simple, performant and scalable Jax LLM!
* [Megatron-DeepSpeed](https://github.com/microsoft/Megatron-DeepSpeed) ⭐ 2,262 | 🐛 162 | 🌐 Python | 📅 2025-08-14 - DeepSpeed version of NVIDIA's Megatron-LM that adds additional support for several features such as MoE model training, Curriculum Learning, 3D Parallelism, and others.
* [Mesh Tensorflow](https://github.com/tensorflow/mesh) ⚠️ Archived - Mesh TensorFlow: Model Parallelism Made Easier.
* [BMTrain](https://github.com/OpenBMB/BMTrain) ⭐ 623 | 🐛 10 | 🌐 Python | 📅 2026-07-07 - Efficient Training for Big Models.
* [TRL](https://huggingface.co/docs/trl/en/index) - TRL is a full stack library where we provide a set of tools to train transformer language models with Reinforcement Learning, from the Supervised Fine-tuning step (SFT), Reward Modeling step (RM) to the Proximal Policy Optimization (PPO) step.

</details>

## LLM Inference

> Reference: [llm-inference-solutions](https://github.com/mani-kantap/llm-inference-solutions) ⭐ 95 | 🐛 1 | 📅 2025-03-01

* [ollama](https://github.com/ollama/ollama) ⭐ 180,229 | 🐛 3,903 | 🌐 Go | 📅 2026-09-05 - Get up and running with Llama 3, Mistral, Gemma, and other large language models.
* [llama.cpp](https://github.com/ggerganov/llama.cpp) ⭐ 127,146 | 🐛 2,420 | 🌐 C++ | 📅 2026-09-05 - LLM inference in C/C++.
* [vLLM](https://github.com/vllm-project/vllm) ⭐ 91,030 | 🐛 7,584 | 🌐 Python | 📅 2026-09-05 - A high-throughput and memory-efficient inference and serving engine for LLMs.
* [SGLang](https://github.com/sgl-project/sglang) ⭐ 35,507 | 🐛 5,160 | 🌐 Python | 📅 2026-09-05 - SGLang is a fast serving framework for large language models and vision language models.
* [TensorRT-LLM](https://github.com/NVIDIA/TensorRT-LLM) ⭐ 14,552 | 🐛 1,447 | 🌐 Python | 📅 2026-09-05 - Nvidia Framework for LLM Inference
* [TGI](https://huggingface.co/docs/text-generation-inference/en/index) - a toolkit for deploying and serving Large Language Models (LLMs).

<details>
<summary>other deployment tools</summary>

* [FastChat](https://github.com/lm-sys/FastChat) ⭐ 39,526 | 🐛 1,046 | 🌐 Python | 📅 2026-05-01 - A distributed multi-model LLM serving system with web UI and OpenAI-compatible RESTful APIs.
* [OpenLLM](https://github.com/bentoml/OpenLLM) ⭐ 12,526 | 🐛 17 | 🌐 Python | 📅 2026-08-31 - Fine-tune, serve, deploy, and monitor any open-source LLMs in production. Used in production at [BentoML](https://bentoml.com/) for LLMs-based applications.
* [SkyPilot](https://github.com/skypilot-org/skypilot) ⭐ 10,563 | 🐛 392 | 🌐 Python | 📅 2026-09-05 - Run LLMs and batch jobs on any cloud. Get maximum cost savings, highest GPU availability, and managed execution -- all with a simple interface.
* [LMDeploy](https://github.com/InternLM/lmdeploy) ⭐ 8,042 | 🐛 608 | 🌐 Python | 📅 2026-09-05 - A high-throughput and low-latency inference and serving framework for LLMs and VLs
* [mistral.rs](https://github.com/EricLBuehler/mistral.rs) ⭐ 7,657 | 🐛 368 | 🌐 Rust | 📅 2026-09-04 - Blazingly fast LLM inference.
* [Liger-Kernel](https://github.com/linkedin/Liger-Kernel) ⭐ 6,599 | 🐛 215 | 🌐 Python | 📅 2026-09-03 - Efficient Triton Kernels for LLM Training.
* [FasterTransformer](https://github.com/NVIDIA/FasterTransformer) ⭐ 6,447 | 🐛 289 | 🌐 C++ | 📅 2024-03-27 - NVIDIA Framework for LLM Inference(Transitioned to TensorRT-LLM)
* [Text-Embeddings-Inference](https://github.com/huggingface/text-embeddings-inference) ⭐ 5,040 | 🐛 210 | 🌐 Rust | 📅 2026-07-24 - Inference for text-embeddings in Rust, HFOIL Licence.
* [exllama](https://github.com/turboderp/exllama) ⭐ 2,941 | 🐛 65 | 🌐 Python | 📅 2023-09-30 - A more memory-efficient rewrite of the HF transformers implementation of Llama for use with quantized weights.
* [Infinity](https://github.com/michaelfeil/infinity) ⭐ 2,932 | 🐛 134 | 🌐 Python | 📅 2026-03-24 - Inference for text-embeddings in Python
* [DeepSpeed-Mii](https://github.com/microsoft/DeepSpeed-MII) ⭐ 2,112 | 🐛 209 | 🌐 Python | 📅 2025-06-30 -  MII makes low-latency and high-throughput inference, similar to vLLM powered by DeepSpeed.
* [MInference](https://github.com/microsoft/MInference) ⭐ 1,227 | 🐛 93 | 🌐 Python | 📅 2026-04-08 - To speed up Long-context LLMs' inference, approximate and dynamic sparse calculate the attention, which reduces inference latency by up to 10x for pre-filling on an A100 while maintaining accuracy.
* [deploy-llms-with-ansible](https://github.com/xamey/deploy-llms-with-ansible) ⭐ 3 | 🐛 0 | 📅 2025-05-01 - Easily deploy any LLM on a VM with minimal configuration, using Ansible.
* [Haystack](https://haystack.deepset.ai/) - an open-source NLP framework that allows you to use LLMs and transformer-based models from Hugging Face, OpenAI and Cohere to interact with your own data.
* [prima.cpp](https://github.com/Lizonghang/prima.cpp) - A distributed implementation of llama.cpp that lets you run 70B-level LLMs on your everyday devices.

</details>

## LLM Applications

> Reference: [awesome-llm-apps](https://github.com/Shubhamsaboo/awesome-llm-apps) ⭐ 136,185 | 🐛 7 | 🌐 Python | 📅 2026-09-02

* [LangChain](https://github.com/hwchase17/langchain) ⭐ 145,703 | 🐛 453 | 🌐 Python | 📅 2026-09-05 — A popular Python/JavaScript library for chaining sequences of language model prompts.
* [LlamaIndex](https://github.com/jerryjliu/llama_index) ⭐ 52,030 | 🐛 705 | 🌐 Python | 📅 2026-09-05 — A Python library for augmenting LLM apps with data.
* [dspy](https://github.com/stanfordnlp/dspy) ⭐ 37,790 | 🐛 652 | 🌐 Python | 📅 2026-09-05 - DSPy: The framework for programming—not prompting—foundation models.

<details>
<summary>more applications</summary>

* [Dify](https://github.com/langgenius/dify) ⭐ 154,518 | 🐛 1,040 | 🌐 TypeScript | 📅 2026-09-05 - An open-source LLM app development platform with an intuitive interface that streamlines AI workflows, model management, and production deployment.

* [Embedchain](https://github.com/embedchain/embedchain) ⭐ 64,738 | 🐛 729 | 🌐 Python | 📅 2026-09-04 - Framework to create ChatGPT like bots over your dataset.

* [Langchain-Chatchat](https://github.com/chatchat-space/Langchain-Chatchat) ⭐ 38,613 | 🐛 27 | 🌐 Python | 📅 2025-11-10 - Formerly langchain-ChatGLM, local knowledge based LLM (like ChatGLM) QA app with langchain.

* [Langfuse](https://github.com/langfuse/langfuse) ⭐ 34,228 | 🐛 907 | 🌐 TypeScript | 📅 2026-09-05 -  Open Source LLM Engineering Platform 🪢 Tracing, Evaluations, Prompt Management, Evaluations and Playground.

* [Semantic Kernel](https://github.com/microsoft/semantic-kernel) ⭐ 28,535 | 🐛 282 | 🌐 C# | 📅 2026-09-04 — A Python/C#/Java library from Microsoft that supports prompt templating, function chaining, vectorized memory, and intelligent planning.

* [promptfoo](https://github.com/typpo/promptfoo) ⭐ 24,841 | 🐛 575 | 🌐 TypeScript | 📅 2026-09-05 - Test your prompts. Evaluate and compare LLM outputs, catch regressions, and improve prompt quality.

* [Opik](https://github.com/comet-ml/opik) ⭐ 21,812 | 🐛 256 | 🌐 Python | 📅 2026-09-05 - Confidently evaluate, test, and ship LLM applications with a suite of observability tools to calibrate language model outputs across your dev and production lifecycle.

* [Guidance](https://github.com/microsoft/guidance) ⭐ 21,737 | 🐛 323 | 🌐 Jupyter Notebook | 📅 2026-05-21 — A handy looking Python library from Microsoft that uses Handlebars templating to interleave generation, prompting, and logical control.

* [OpenAI Evals](https://github.com/openai/evals) ⭐ 19,387 | 🐛 331 | 🌐 Python | 📅 2026-04-14 — An open-source library for evaluating task performance of language models and prompts.

* [MNN-LLM](https://github.com/alibaba/MNN) ⭐ 16,029 | 🐛 48 | 🌐 C++ | 📅 2026-09-04 -- A Device-Inference framework, including LLM Inference on device(Mobile Phone/PC/IOT)

* [Outlines](https://github.com/normal-computing/outlines) ⭐ 15,750 | 🐛 160 | 🌐 Python | 📅 2026-09-04 — A Python library that provides a domain-specific language to simplify prompting and constrain generation.

* [wechat-chatgpt](https://github.com/fuergaosi233/wechat-chatgpt) ⭐ 13,240 | 🐛 53 | 🌐 TypeScript | 📅 2024-05-20 - Use ChatGPT On Wechat via wechaty

* [AI Gateway](https://github.com/Portkey-AI/gateway) ⭐ 12,905 | 🐛 258 | 🌐 TypeScript | 📅 2026-05-25 — Gateway streamlines requests to 100+ open & closed source models with a unified API. It is also production-ready with support for caching, fallbacks, retries, timeouts, loadbalancing, and can be edge-deployed for minimum latency.

* [Search with Lepton](https://github.com/leptonai/search_with_lepton) ⚠️ Archived - Build your own conversational search engine using less than 500 lines of code by [LeptonAI](https://github.com/leptonai).

* [Evidently](https://github.com/evidentlyai/evidently) ⭐ 7,891 | 🐛 302 | 🌐 Jupyter Notebook | 📅 2026-08-31 — An open-source framework to evaluate, test and monitor ML and LLM-powered systems.

* [LLocalSearch](https://github.com/nilsherzig/LLocalSearch) ⚠️ Archived - Locally running websearch using LLM chains

* [Serge](https://github.com/serge-chat/serge) ⚠️ Archived - a chat interface crafted with llama.cpp for running Alpaca models. No API keys, entirely self-hosted!

* [GPUStack](https://github.com/gpustack/gpustack) ⭐ 5,609 | 🐛 680 | 🌐 Python | 📅 2026-09-02 - An open-source GPU cluster manager for running LLMs

* [AutoRAG](https://github.com/Marker-Inc-Korea/AutoRAG) ⭐ 5,059 | 🐛 119 | 🌐 TypeScript | 📅 2026-09-05 - Open source AutoML tool for RAG. Optimize the RAG answer quality automatically. From generation evaluation datset to deploying optimized RAG pipeline.

* [Agenta](https://github.com/agenta-ai/agenta) ⭐ 4,685 | 🐛 316 | 🌐 TypeScript | 📅 2026-09-05 -  Easily build, version, evaluate and deploy your LLM-powered apps.

* [Promptify](https://github.com/promptslab/Promptify) ⭐ 4,638 | 🐛 60 | 🌐 Python | 📅 2026-03-27 — A small Python library for using language models to perform NLP tasks.

* [AdalFlow](https://github.com/SylphAI-Inc/AdalFlow) ⭐ 4,213 | 🐛 68 | 🌐 Python | 📅 2026-05-29 - AdalFlow: The library to build\&auto-optimize LLM applications.

* [Langroid](https://github.com/langroid/langroid) ⭐ 4,102 | 🐛 52 | 🌐 Python | 📅 2026-09-05 - Harness LLMs with Multi-Agent Programming

* [LazyLLM](https://github.com/LazyAGI/LazyLLM) ⭐ 3,880 | 🐛 45 | 🌐 Python | 📅 2026-09-04 - An open-source LLM app for building multi-agent LLMs applications in an easy and lazy way, supports model deployment and fine-tuning.

* [LangWatch](https://github.com/langwatch/langwatch) ⭐ 3,523 | 🐛 925 | 🌐 TypeScript | 📅 2026-09-05 - Open-source LLM observability, prompt evaulation, and prompt optimzation platform.

* [Prompttools](https://github.com/hegelai/prompttools) ⭐ 3,053 | 🐛 43 | 🌐 Python | 📅 2026-02-11 — Open-source Python tools for testing and evaluating models, vector DBs, and prompts.

* [magentic](https://github.com/jackmpcollins/magentic) ⭐ 2,421 | 🐛 50 | 🌐 Python | 📅 2026-03-11 - Seamlessly integrate LLMs as Python functions

* [llm-ui](https://github.com/llm-ui-kit/llm-ui) ⭐ 1,743 | 🐛 16 | 🌐 TypeScript | 📅 2025-07-02 - A React library for building LLM UIs.

* [MemFree](https://github.com/memfreeme/memfree) ⭐ 1,506 | 🐛 19 | 🌐 TypeScript | 📅 2026-07-06 - Open Source Hybrid AI Search Engine, Instantly Get Accurate Answers from the Internet, Bookmarks, Notes, and Docs. Support One-Click Deployment

* [ModelFusion](https://github.com/lgrammel/modelfusion) ⚠️ Archived - A TypeScript library for building apps with LLMs and other ML models (speech-to-text, text-to-speech, image generation).

* [Wllama](https://github.com/ngxson/wllama) ⭐ 1,195 | 🐛 46 | 🌐 TypeScript | 📅 2026-09-03 - WebAssembly binding for llama.cpp - Enabling in-browser LLM inference

* [Swiss Army Llama](https://github.com/Dicklesworthstone/swiss_army_llama) ⭐ 1,055 | 🐛 0 | 🌐 Python | 📅 2025-02-27 - Comprehensive set of tools for working with local LLMs for various tasks.

* [Agentic Radar](https://github.com/splx-ai/agentic-radar) ⭐ 1,046 | 🐛 15 | 🌐 Python | 📅 2025-11-27 - Open-source CLI security scanner for agentic workflows. Scans your workflow’s source code, detects vulnerabilities, and generates an interactive visualization along with a detailed security report. Supports LangGraph, CrewAI, n8n, OpenAI Agents, and more.

* [Robocorp](https://github.com/robocorp/robocorp) ⭐ 650 | 🐛 11 | 🌐 Python | 📅 2026-09-01 - Create, deploy and operate Actions using Python anywhere to enhance your AI agents and assistants. Batteries included with an extensive set of libraries, helpers and logging.

* [MindSQL](https://github.com/Mindinventory/MindSQL) ⭐ 448 | 🐛 10 | 🌐 Python | 📅 2025-07-16 - A python package for Txt-to-SQL with self hosting functionalities and RESTful APIs compatible with proprietary as well as open source LLM.

* [talkd.ai dialog](https://github.com/talkdai/dialog) ⭐ 427 | 🐛 23 | 🌐 Python | 📅 2024-12-18 - Simple API for deploying any RAG or LLM that you want adding plugins.

* [LiteChain](https://github.com/rogeriochaves/litechain) ⭐ 417 | 🐛 3 | 🌐 Python | 📅 2024-01-03 - Lightweight alternative to LangChain for composing LLMs

* [QA-Pilot](https://github.com/reid41/QA-Pilot) ⭐ 326 | 🐛 8 | 🌐 Svelte | 📅 2026-09-04 - An interactive chat project that leverages Ollama/OpenAI/MistralAI LLMs for rapid understanding and navigation of GitHub code repository or compressed file resources.

* [Shell-Pilot](https://github.com/reid41/shell-pilot) ⭐ 117 | 🐛 2 | 🌐 Shell | 📅 2025-01-28 - Interact with LLM using Ollama models(or openAI, mistralAI)via pure shell scripts on your Linux(or MacOS) system, enhancing intelligent system management without any dependencies.

* [Just-Chat](https://github.com/longevity-genie/just-chat) ⭐ 79 | 🐛 2 | 🌐 Python | 📅 2025-11-22 - Make your LLM agent and chat with it simple and fast!

* [IntelliServer](https://github.com/intelligentnode/IntelliServer) ⭐ 29 | 🐛 2 | 🌐 JavaScript | 📅 2026-07-13 - simplifies the evaluation of LLMs by providing a unified microservice to access and test multiple AI models.

* [MLflow](https://mlflow.org/) - MLflow: An open-source framework for the end-to-end machine learning lifecycle, helping developers track experiments, evaluate models/prompts, deploy models, and add observability with tracing.

* [Tune Studio](https://studio.tune.app/) - Playground for devs to finetune & deploy LLMs

* [CAMEL](https://www.camel-ai.org/) - First LLM Multi-agent framework.

* [Chainlit](https://docs.chainlit.io/overview) — A Python library for making chatbot interfaces.

* [Guardrails.ai](https://www.guardrailsai.com/docs/) — A Python library for validating outputs and retrying failures. Still in alpha, so expect sharp edges and bugs.

* [Scale Spellbook](https://scale.com/spellbook) — A paid product for building, comparing, and shipping language model apps.

* [PromptPerfect](https://promptperfect.jina.ai/prompts) — A paid product for testing and improving prompts.

* [Weights & Biases](https://wandb.ai/site/solutions/llmops) — A paid product for tracking model training and prompt engineering experiments.

* [Arthur Shield](https://www.arthur.ai/get-started) — A paid product for detecting toxicity, hallucination, prompt injection, etc.

* [LMQL](https://lmql.ai) — A programming language for LLM interaction with support for typed prompting, control flow, constraints, and tools.

* [OneKE](https://openspg.yuque.com/ndx6g9/ps5q6b/vfoi61ks3mqwygvy) — A bilingual Chinese-English knowledge extraction model with knowledge graphs and natural language processing technologies.

* [Wordware](https://www.wordware.ai) - A web-hosted IDE where non-technical domain experts work with AI Engineers to build task-specific AI agents. We approach prompting as a new programming language rather than low/no-code blocks.

* [Wallaroo.AI](https://github.com/WallarooLabs) - Deploy, manage, optimize any model at scale across any environment from cloud to edge. Let's you go from python notebook to inferencing in minutes.

* [Epsilla](https://github.com/epsilla-cloud) - An all-in-one LLM Agent platform with your private data and knowledge, delivers your production-ready AI Agents on Day 1.

* [Arize-Phoenix](https://phoenix.arize.com/) - Open-source tool for ML observability that runs in your notebook environment. Monitor and fine tune LLM, CV and Tabular Models.

* [LLM](\[https://github.com/simonw/llm) - A CLI utility and Python library for interacting with Large Language Models, both via remote APIs and models that can be installed and run on your own machine.

* [TensorZero](https://www.tensorzero.com/) - TensorZero is an open-source framework for building production-grade LLM applications. It unifies an LLM gateway, observability, optimization, evaluations, and experimentation.

</details>

## LLM Tutorials and Courses

* [llm-course](https://github.com/mlabonne/llm-course) ⭐ 82,320 | 🐛 91 | 📅 2026-02-05 - Course to get into Large Language Models (LLMs) with roadmaps and Colab notebooks.
* [LLM‑RL‑Visualized (EN)](https://github.com/changyeyu/LLM-RL-Visualized/blob/master/src/README_EN.md) ⭐ 4,847 | 🐛 3 | 🌐 Python | 📅 2026-08-29 | [LLM‑RL‑Visualized (中文)](https://github.com/changyeyu/LLM-RL-Visualized) ⭐ 4,847 | 🐛 3 | 🌐 Python | 📅 2026-08-29 - 100+  LLM / RL Algorithm Maps📚.
* [femtoGPT](https://github.com/keyvank/femtoGPT) ⭐ 937 | 🐛 10 | 🌐 Rust | 📅 2025-10-21 - Pure Rust implementation of a minimal Generative Pretrained Transformer.
* [Andrej Karpathy Series](https://www.youtube.com/@AndrejKarpathy) - My favorite!
* [Umar Jamil Series](https://www.youtube.com/@umarjamilai) - high quality and educational videos you don't want to miss.
* [Alexander Rush Series](https://rush-nlp.com/projects/) - high quality and educational materials you don't want to miss.
* [UWaterloo CS 886](https://cs.uwaterloo.ca/~wenhuche/teaching/cs886/) - Recent Advances on Foundation Models.
* [CS25-Transformers United](https://web.stanford.edu/class/cs25/)
* [ChatGPT Prompt Engineering](https://www.deeplearning.ai/short-courses/chatgpt-prompt-engineering-for-developers/)
* [Princeton: Understanding Large Language Models](https://www.cs.princeton.edu/courses/archive/fall22/cos597G/)
* [CS324 - Large Language Models](https://stanford-cs324.github.io/winter2022/)
* [State of GPT](https://build.microsoft.com/en-US/sessions/db3f4859-cd30-4445-a0cd-553c3304f8e2)
* [A Visual Guide to Mamba and State Space Models](https://maartengrootendorst.substack.com/p/a-visual-guide-to-mamba-and-state?utm_source=multiple-personal-recommendations-email\&utm_medium=email\&open=false)
* [Let's build GPT: from scratch, in code, spelled out.](https://www.youtube.com/watch?v=kCc8FmEb1nY)
* [minbpe](https://www.youtube.com/watch?v=zduSFxRajkE\&t=1157s) - Minimal, clean code for the Byte Pair Encoding (BPE) algorithm commonly used in LLM tokenization.
* [Neurips2022-Foundational Robustness of Foundation Models](https://nips.cc/virtual/2022/tutorial/55796)
* [ICML2022-Welcome to the "Big Model" Era: Techniques and Systems to Train and Serve Bigger Models](https://icml.cc/virtual/2022/tutorial/18440)
* [GPT in 60 Lines of NumPy](https://jaykmody.com/blog/gpt-from-scratch/)

## LLM Books

* [Generative AI with LangChain: Build large language model (LLM) apps with Python, ChatGPT, and other LLMs](https://amzn.to/3GUlRng) - it comes with a [GitHub repository](https://github.com/benman1/generative_ai_with_langchain) ⭐ 1,413 | 🐛 0 | 🌐 Jupyter Notebook | 📅 2026-08-14 that showcases a lot of the functionality
* [Build a Large Language Model (From Scratch)](https://www.manning.com/books/build-a-large-language-model-from-scratch) - A guide to building your own working LLM.
* [BUILD GPT: HOW AI WORKS](https://www.amazon.com/dp/9152799727?ref_=cm_sw_r_cp_ud_dp_W3ZHCD6QWM3DPPC0ARTT_1) - explains how to code a Generative Pre-trained Transformer, or GPT, from scratch.
* [Hands-On Large Language Models: Language Understanding and Generation](https://www.llm-book.com/) - Explore the world of Large Language Models with over 275 custom made figures in this illustrated guide!
* [The Chinese Book for Large Language Models](http://aibox.ruc.edu.cn/zws/index.htm) - An Introductory LLM Textbook Based on [*A Survey of Large Language Models*](https://arxiv.org/abs/2303.18223).

## Great thoughts about LLM

* [Why did all of the public reproduction of GPT-3 fail?](https://jingfengyang.github.io/gpt)
* [A Stage Review of Instruction Tuning](https://yaofu.notion.site/June-2023-A-Stage-Review-of-Instruction-Tuning-f59dbfc36e2d4e12a33443bd6b2012c2)
* [LLM Powered Autonomous Agents](https://lilianweng.github.io/posts/2023-06-23-agent/)
* [Why you should work on AI AGENTS!](https://www.youtube.com/watch?v=fqVLjtvWgq8)
* [Google "We Have No Moat, And Neither Does OpenAI"](https://www.semianalysis.com/p/google-we-have-no-moat-and-neither)
* [AI competition statement](https://petergabriel.com/news/ai-competition-statement/)
* [Prompt Engineering](https://lilianweng.github.io/posts/2023-03-15-prompt-engineering/)
* [Noam Chomsky: The False Promise of ChatGPT](https://www.nytimes.com/2023/03/08/opinion/noam-chomsky-chatgpt-ai.html)
* [Is ChatGPT 175 Billion Parameters? Technical Analysis](https://orenleung.super.site/is-chatgpt-175-billion-parameters-technical-analysis)
* [The Next Generation Of Large Language Models ](https://www.notion.so/Awesome-LLM-40c8aa3f2b444ecc82b79ae8bbd2696b)
* [Large Language Model Training in 2023](https://research.aimultiple.com/large-language-model-training/)
* [How does GPT Obtain its Ability? Tracing Emergent Abilities of Language Models to their Sources](https://yaofu.notion.site/How-does-GPT-Obtain-its-Ability-Tracing-Emergent-Abilities-of-Language-Models-to-their-Sources-b9a57ac0fcf74f30a1ab9e3e36fa1dc1)
* [Open Pretrained Transformers](https://www.youtube.com/watch?v=p9IxoSkvZ-M\&t=4s)
* [Scaling, emergence, and reasoning in large language models](https://docs.google.com/presentation/d/1EUV7W7X_w0BDrscDhPg7lMGzJCkeaPkGCJ3bN8dluXc/edit?pli=1\&resourcekey=0-7Nz5A7y8JozyVrnDtcEKJA#slide=id.g16197112905_0_0)

## Miscellaneous

* [AutoGPT](https://github.com/Significant-Gravitas/Auto-GPT) ⭐ 187,151 | 🐛 563 | 🌐 Python | 📅 2026-09-05 - an experimental open-source application showcasing the capabilities of the GPT-4 language model.
* [chatgpt-wrapper](https://github.com/mmabrouk/chatgpt-wrapper) ⭐ 3,715 | 🐛 3 | 🌐 Python | 📅 2026-09-04 - ChatGPT Wrapper is an open-source unofficial Python API and CLI that lets you interact with ChatGPT.
* [EasyEdit](https://github.com/zjunlp/EasyEdit) ⭐ 2,911 | 🐛 1 | 🌐 Jupyter Notebook | 📅 2026-07-14 - An easy-to-use framework to edit large language models.
* [OpenAGI](https://github.com/agiresearch/OpenAGI) ⭐ 2,282 | 🐛 10 | 🌐 Python | 📅 2024-11-28 - When LLM Meets Domain Experts.
* [chatgpt-shroud](https://github.com/guyShilo/chatgpt-shroud) ⭐ 10 | 🐛 0 | 🌐 JavaScript | 📅 2023-05-28 - A Chrome extension for OpenAI's ChatGPT, enhancing user privacy by enabling easy hiding and unhiding of chat history. Ideal for privacy during screen shares.
* [Emergent Mind](https://www.emergentmind.com) - The latest AI news, curated & explained by GPT-4.
* [ShareGPT](https://sharegpt.com) - Share your wildest ChatGPT conversations with one click.
* [Major LLMs + Data Availability](https://docs.google.com/spreadsheets/d/1bmpDdLZxvTCleLGVPgzoMTQ0iDP2-7v7QziPrzPdHyM/edit#gid=0)
* [500+ Best AI Tools](https://vaulted-polonium-23c.notion.site/500-Best-AI-Tools-e954b36bf688404ababf74a13f98d126)
* [Cohere Summarize Beta](https://txt.cohere.ai/summarize-beta/) - Introducing Cohere Summarize Beta: A New Endpoint for Text Summarization
* [Cursor](https://www.cursor.so) - Write, edit, and chat about your code with a powerful AI.
* [AI For Developers](https://aifordevelopers.org) - List of AI Tools and Agents for Developers

## Contributing

This is an active repository and your contributions are always welcome!

I will keep some pull requests open if I'm not sure if they are awesome for LLM, you could vote for them by adding 👍 to them.

***

If you have any question about this opinionated list, do not hesitate to contact me <chengxin1998@stu.pku.edu.cn>.

[^1]: This is not legal advice. Please contact the original authors of the models for more information.

***

> _Enhansomed by [enhansome](https://github.com/enhansome) on 2026-09-05._
