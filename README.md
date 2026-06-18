# Awesome Data Problems for Foundation Models

> A curated reading list on data problems for foundation models, inspired by the DATA-FM / DPFM workshops and Awesome-style paper repositories.

Foundation models are increasingly limited, shaped, and governed by their data: how it is collected, filtered, mixed, valued, attributed, protected, evaluated, and regenerated. This repository tracks recent papers, datasets, benchmarks, and position work on **data-centric foundation model research**, with an emphasis on work from 2023 onward.

## Scope

The taxonomy follows the DATA-FM workshop themes: data collection and curation, data attribution and valuation, legal/copyright and privacy, synthetic data and model collapse, safety/fairness, and benchmark contamination/evaluation. Borderline papers are included when their main contribution changes how data is sourced, selected, audited, or evaluated for foundation models.


## Badge Convention

Paper badges use the format `year-venue/source-color`. They reflect the latest known formal venue/source checked from official proceedings, arXiv metadata, or bibliographic search as of 2026-06-18; entries remain `arXiv`, `Survey`, `Dataset`, or `Resource` when no reliable formal venue was found.

## Contents

- [Badge Convention](#badge-convention)
- [Surveys and Position Papers](#surveys-and-position-papers)
- [Open Corpora, Recipes, and Data-Centric Model Releases](#open-corpora-recipes-and-data-centric-model-releases)
- [Pretraining Data Selection, Filtering, and Mixing](#pretraining-data-selection-filtering-and-mixing)
- [Instruction, Preference, and Alignment Data](#instruction-preference-and-alignment-data)
- [Continual Learning and Replay Data](#continual-learning-and-replay-data)
- [Synthetic Data and Model Collapse](#synthetic-data-and-model-collapse)
- [Data Attribution, Valuation, and Influence](#data-attribution-valuation-and-influence)
- [Privacy, Copyright, Consent, and Unlearning](#privacy-copyright-consent-and-unlearning)
- [Benchmark Contamination, Freshness, and RAG Evaluation](#benchmark-contamination-freshness-and-rag-evaluation)
- [Multimodal and Vision-Language Data](#multimodal-and-vision-language-data)
- [Safety, Fairness, and Data Poisoning](#safety-fairness-and-data-poisoning)
- [Classic References](#classic-references)
- [Related Workshops and Resources](#related-workshops-and-resources)

## Surveys and Position Papers

- ![2025 Survey](https://img.shields.io/badge/2025-Survey-9cf) [Rethinking Data Mixture for Large Language Models: A Comprehensive Survey and New Perspectives](https://arxiv.org/abs/2505.21598) - Survey of offline/online data mixture optimization.
- ![2025 Survey](https://img.shields.io/badge/2025-Survey-9cf) [A Survey on Data Contamination for Large Language Models](https://arxiv.org/abs/2502.14425) - Survey of contamination-free evaluation and contamination detection.
- ![2025 Survey](https://img.shields.io/badge/2025-Survey-9cf) [A Survey on Efficient Large Language Model Training: From Data-centric Perspectives](https://arxiv.org/abs/2510.25817) - Data-efficient post-training taxonomy.
- ![2025 arXiv](https://img.shields.io/badge/2025-arXiv-lightgrey) [Ten Challenging Problems in Federated Foundation Models](https://arxiv.org/abs/2502.12176) - Includes private data, heterogeneity, unlearning, incentives, and privacy in FedFMs.
- ![2024 Survey](https://img.shields.io/badge/2024-Survey-9cf) [A Survey on Data Selection for Language Models](https://arxiv.org/abs/2402.16827) - Broad taxonomy of LM data selection methods.
- ![2024 Survey](https://img.shields.io/badge/2024-Survey-9cf) [A Survey on Data Synthesis and Augmentation for Large Language Models](https://arxiv.org/abs/2410.12896) - Data synthesis across pretraining, instruction tuning, and preference learning.
- ![2024 Survey](https://img.shields.io/badge/2024-Survey-9cf) [Data-Centric Foundation Models in Computational Healthcare: A Survey](https://arxiv.org/abs/2401.02458) - Healthcare-specific data quality, privacy, annotation, and ethics.
- ![2024 Survey](https://img.shields.io/badge/2024-Survey-9cf) [Benchmark Data Contamination of Large Language Models: A Survey](https://arxiv.org/abs/2406.04244) - Benchmark contamination risks and mitigations.
- ![2023 Survey](https://img.shields.io/badge/2023-Survey-9cf) [Data-centric Artificial Intelligence: A Survey](https://arxiv.org/abs/2303.10158) - General data-centric AI lifecycle survey.

## Open Corpora, Recipes, and Data-Centric Model Releases

- ![2026 arXiv](https://img.shields.io/badge/2026-arXiv-lightgrey) [How2Everything: Mining the Web for How-To Procedures to Evaluate and Improve LLMs](https://arxiv.org/abs/2602.08808) - Web-mined procedural data, benchmark, scoring, and RL loop.
- ![2025 Dataset](https://img.shields.io/badge/2025-Dataset-yellow) [The Common Pile v0.1: An 8TB Dataset of Public Domain and Openly Licensed Text](https://arxiv.org/abs/2506.05209) - Public-domain/openly licensed pretraining corpus and Comma models.
- ![2025 Resource](https://img.shields.io/badge/2025-Resource-informational) [FlexOlmo: Open Language Models for Flexible Data Use](https://arxiv.org/abs/2507.07024) - Modular data ownership and inference-time inclusion/exclusion of data experts.
- ![2026 ICML](https://img.shields.io/badge/2026-ICML-blue) [MixtureVitae: Open Web-Scale Pretraining Dataset With High Quality Instruction and Reasoning Data Built from Permissive-First Text Sources](https://arxiv.org/abs/2509.25531) - Permissive-first pretraining corpus with provenance-aware curation recipes.
- ![2025 Resource](https://img.shields.io/badge/2025-Resource-informational) [2 OLMo 2 Furious](https://arxiv.org/abs/2501.00656) - Fully open OLMo 2 recipes, staged data mixtures, and instruction data.
- ![2024 Resource](https://img.shields.io/badge/2024-Resource-informational) [OLMo: Accelerating the Science of Language Models](https://arxiv.org/abs/2402.00838) - Open model release with training data, logs, code, and checkpoints.
- ![2024 Dataset](https://img.shields.io/badge/2024-Dataset-yellow) [Dolma: an Open Corpus of Three Trillion Tokens for Language Model Pretraining Research](https://arxiv.org/abs/2402.00159) - Open corpus and curation toolkit.
- ![2024 Dataset](https://img.shields.io/badge/2024-Dataset-yellow) [The FineWeb Datasets: Decanting the Web for the Finest Text Data at Scale](https://arxiv.org/abs/2406.17557) - 15T-token web corpus plus filtering/deduplication ablations.
- ![2024 Dataset](https://img.shields.io/badge/2024-Dataset-yellow) [DataComp-LM: In search of the next generation of training sets for language models](https://arxiv.org/abs/2406.11794) - Standardized benchmark for LM dataset experiments.
- ![2023 Dataset](https://img.shields.io/badge/2023-Dataset-yellow) [CulturaX: A Cleaned, Enormous, and Multilingual Dataset for Large Language Models in 167 Languages](https://arxiv.org/abs/2309.09400) - Multilingual cleaned and deduplicated corpus.
- ![2023 Dataset](https://img.shields.io/badge/2023-Dataset-yellow) [The RefinedWeb Dataset for Falcon LLM](https://arxiv.org/abs/2306.01116) - Web-only filtered/deduplicated corpus for Falcon.
- ![2023 Dataset](https://img.shields.io/badge/2023-Dataset-yellow) [DataComp: In search of the next generation of multimodal datasets](https://arxiv.org/abs/2304.14108) - Multimodal data curation benchmark for CLIP-style training.

## Pretraining Data Selection, Filtering, and Mixing

- ![2025 ICML](https://img.shields.io/badge/2025-ICML-blue) [Organize the Web: Constructing Domains Enhances Pre-Training Data Curation](https://arxiv.org/abs/2502.10341) - Topic/format domain construction for web corpora.
- ![2025 DATA-FM](https://img.shields.io/badge/2025-DATA--FM-orange) [Data Mixing Can Induce Phase Transitions in Knowledge Acquisition](https://openreview.net/forum?id=ZKA4yiGdrA) - DATA-FM 2025 oral on knowledge-dense mixtures and thresholds.
- ![2025 ICML](https://img.shields.io/badge/2025-ICML-blue) [MASS: Mathematical Data Selection via Skill Graphs for Pretraining Large Language Models](https://arxiv.org/abs/2503.14917) - Skill-graph-based mathematical data selection.
- ![2025 arXiv](https://img.shields.io/badge/2025-arXiv-lightgrey) [TiKMiX: Take Data Influence into Dynamic Mixture for Language Model Pre-training](https://arxiv.org/abs/2508.17677) - Dynamic mixture optimization via group influence.
- ![2026 ICML](https://img.shields.io/badge/2026-ICML-blue) [Active Learning with Low-Rank Structure for Data Selection](https://arxiv.org/abs/2606.16045) - Low-rank active learning formulation for representative subset selection.
- ![2026 ICML](https://img.shields.io/badge/2026-ICML-blue) [InfoLaw: Information Scaling Laws for Large Language Models with Quality-Weighted Mixture Data and Repetition](https://arxiv.org/abs/2605.02364) - Data-aware scaling law for mixture quality, repetition, and overtraining.
- ![2026 ICML](https://img.shields.io/badge/2026-ICML-blue) [Capacity-Aware Mixture Law Enables Efficient LLM Data Optimization](https://arxiv.org/abs/2603.08022) - Predicts target-model performance for compute-efficient LLM data mixture search.
- ![2026 ICML](https://img.shields.io/badge/2026-ICML-blue) [BLISS: A Lightweight Bilevel Influence Scoring Method for Data Selection in Language Model Pretraining](https://arxiv.org/abs/2510.06048) - Bilevel influence scoring for from-scratch LLM pretraining data selection.
- ![2026 ICML](https://img.shields.io/badge/2026-ICML-blue) [GEM: Geometric Entropy Mixing for Optimal LLM Data Curation](https://arxiv.org/abs/2605.26121) - Geometric entropy objective for semantic data mixing and taxonomy construction.
- ![2026 ICML](https://img.shields.io/badge/2026-ICML-blue) [Target-Oriented Pretraining Data Selection via Neuron-Activated Graph](https://arxiv.org/abs/2604.15706) - Training-free target-domain data selection using neuron activation graphs.
- ![2026 ICML](https://img.shields.io/badge/2026-ICML-blue) [MergeMix: Optimizing Mid-Training Data Mixtures via Learnable Model Merging](https://arxiv.org/abs/2601.17858) - Uses model merging weights as a low-cost proxy for mid-training data mixture optimization.
- ![2026 ICML](https://img.shields.io/badge/2026-ICML-blue) [D$^3$: Dynamic Directional Graph-Constrained Data Scheduling for LLM Training](https://arxiv.org/abs/2605.31164) - Dynamic influence-graph scheduling for LLM training data order.
- ![2026 ICML](https://img.shields.io/badge/2026-ICML-blue) [OPUS: Towards Efficient and Principled Data Selection in Large Language Model Pre-training in Every Iteration](https://arxiv.org/abs/2602.05400) - Optimizer-induced utility selection for token-level pretraining efficiency.
- ![2026 ICML](https://img.shields.io/badge/2026-ICML-blue) [Procedural Pretraining: Warming Up Language Models with Abstract Data](https://arxiv.org/abs/2601.21725) - Front-loads abstract procedural data to improve downstream LM pretraining efficiency.
- ![2026 ICML](https://img.shields.io/badge/2026-ICML-blue) [Understanding Data Temporality Impact on Large Language Models Pre-training](https://arxiv.org/abs/2605.22769) - Studies temporally ordered pretraining for factual freshness and time grounding.
- ![2026 ICML](https://img.shields.io/badge/2026-ICML-blue) [When Data Is Scarce: Scaling Sparse Language Models with Repeated Training](https://arxiv.org/abs/2606.01155) - Scaling law for sparse LMs under repeated, data-limited training.
- ![2026 ICML](https://img.shields.io/badge/2026-ICML-blue) [Decouple Searching from Training: Scaling Data Mixing via Model Merging for Large Language Model Pre-training](https://arxiv.org/abs/2602.00747) - Uses model-merging proxies to scale LLM pretraining mixture search.
- ![2026 ICML](https://img.shields.io/badge/2026-ICML-blue) [On the Difficulty of Learning a Meta-network for Training Data Selection](https://arxiv.org/abs/2606.00571) - Analyzes limits of meta-network-based training data selection.
- ![2026 ICML](https://img.shields.io/badge/2026-ICML-blue) [Cram Less to Fit More: Training Data Pruning Improves Memorization of Facts](https://arxiv.org/abs/2604.08519) - Shows pruning can improve fact memorization under training data constraints.
- ![2024 arXiv](https://img.shields.io/badge/2024-arXiv-lightgrey) [Data Mixing Laws: Optimizing Data Mixtures by Predicting Language Modeling Performance](https://arxiv.org/abs/2403.16952) - Predicting performance from mixture proportions.
- ![2024 arXiv](https://img.shields.io/badge/2024-arXiv-lightgrey) [RegMix: Data Mixture as Regression for Language Model Pre-training](https://arxiv.org/abs/2407.01492) - Predicts good mixtures using many small proxy trainings.
- ![2024 arXiv](https://img.shields.io/badge/2024-arXiv-lightgrey) [QuRating: Selecting High-Quality Data for Training Language Models](https://arxiv.org/abs/2402.09739) - LLM-derived quality ratings for pretraining data.
- ![2024 arXiv](https://img.shields.io/badge/2024-arXiv-lightgrey) [Rho-1: Not All Tokens Are What You Need](https://arxiv.org/abs/2404.07965) - Selective language modeling at token level.
- ![2024 arXiv](https://img.shields.io/badge/2024-arXiv-lightgrey) [Data Engineering for Scaling Language Models to 128K Context](https://arxiv.org/abs/2402.10171) - Long-context continual pretraining data recipe.
- ![2024 arXiv](https://img.shields.io/badge/2024-arXiv-lightgrey) [Data Proportion Detection for Optimized Data Management for Large Language Models](https://arxiv.org/abs/2409.17527) - Inferring pretraining data proportions from outputs.
- ![2024 arXiv](https://img.shields.io/badge/2024-arXiv-lightgrey) [Rephrasing natural text data with different languages and quality levels for Large Language Model pre-training](https://arxiv.org/abs/2410.20796) - Rephrasing natural text as pretraining augmentation.
- ![2023 arXiv](https://img.shields.io/badge/2023-arXiv-lightgrey) [DoReMi: Optimizing Data Mixtures Speeds Up Language Model Pretraining](https://arxiv.org/abs/2305.10429) - Domain reweighting with minimax optimization.
- ![2023 NeurIPS](https://img.shields.io/badge/2023-NeurIPS-purple) [Data Selection for Language Models via Importance Resampling](https://arxiv.org/abs/2302.03169) - DSIR data selection using target distribution matching.
- ![2023 arXiv](https://img.shields.io/badge/2023-arXiv-lightgrey) [Skill-it! A Data-Driven Skills Framework for Understanding and Training Language Models](https://arxiv.org/abs/2307.14430) - Skill-aware online sampling and curriculum.

## Instruction, Preference, and Alignment Data

- ![2026 arXiv](https://img.shields.io/badge/2026-arXiv-lightgrey) [How2Everything: Mining the Web for How-To Procedures to Evaluate and Improve LLMs](https://arxiv.org/abs/2602.08808) - Also relevant as procedural instruction data.
- ![2026 ICML](https://img.shields.io/badge/2026-ICML-blue) [TuneAhead: Predicting Fine-tuning Performance Before Full Training Begins](https://arxiv.org/abs/2606.17660) - Predicts LLM fine-tuning outcomes before full training, including data-quality and hyperparameter sensitivity.
- ![2026 ICML](https://img.shields.io/badge/2026-ICML-blue) [The Quality-Utility Paradox: Why High-Reward Data Impairs Small Model Mathematical Reasoning](https://arxiv.org/abs/2606.16152) - Studies when high-reward distillation traces degrade small-model reasoning.
- ![2026 ICML](https://img.shields.io/badge/2026-ICML-blue) [How to Fine-Tune a Reasoning Model? A Teacher-Student Cooperation Framework to Synthesize Student-Consistent SFT Data](https://arxiv.org/abs/2604.14164) - Synthesizes student-consistent reasoning SFT data from teacher-student cooperation.
- ![2026 ICML](https://img.shields.io/badge/2026-ICML-blue) [Training Data Efficiency in Multimodal Process Reward Models](https://arxiv.org/abs/2602.04145) - Studies redundancy and selection criteria for multimodal process reward model data.
- ![2026 ICML](https://img.shields.io/badge/2026-ICML-blue) [AIR: Post-training Data Selection for Reasoning via Attention Head Influence](https://arxiv.org/abs/2512.13279) - Mechanism-guided post-training sample and step selection for reasoning distillation.
- ![2026 ICML](https://img.shields.io/badge/2026-ICML-blue) [ActiveUltraFeedback: Efficient Preference Data Generation using Active Learning](https://arxiv.org/abs/2603.09692) - Active learning pipeline for cheaper, higher-utility preference data.
- ![2026 ICML](https://img.shields.io/badge/2026-ICML-blue) [Differentially Private Preference Data Synthesis for Large Language Model Alignment](https://arxiv.org/abs/2605.30808) - DP synthetic preference data generation for privacy-preserving alignment.
- ![2026 ICML](https://img.shields.io/badge/2026-ICML-blue) [From Parameters to Data: A Task-Parameter-Guided Fine-Tuning Pipeline for Efficient LLM Alignment](https://arxiv.org/abs/2605.21558) - Couples data mining with task-sensitive parameter selection for efficient alignment.
- ![2026 ICML](https://img.shields.io/badge/2026-ICML-blue) [GIST: Targeted Data Selection for Instruction Tuning via Coupled Optimization Geometry](https://arxiv.org/abs/2602.18584) - Instruction data selection via LoRA-aware optimization geometry.
- ![2026 ICML](https://img.shields.io/badge/2026-ICML-blue) [Single-Rollout Hidden-State Dynamics for Training-Free RLVR Data Selection](https://arxiv.org/abs/2605.28631) - Training-free RLVR data selection from hidden-state dynamics.
- ![2026 ICML](https://img.shields.io/badge/2026-ICML-blue) [Theoretical Perspectives on Data Quality and Synergistic Effects in Pre- and Post-Training Reasoning Models](https://arxiv.org/abs/2603.01293) - Theory for how pretraining, SFT, and RL data quality/scale interact in reasoning models.
- ![2026 ICML](https://img.shields.io/badge/2026-ICML-blue) [Less is Enough: Synthesizing Diverse Data in Feature Space of LLMs](https://arxiv.org/abs/2602.10388) - Feature-space synthetic data generation for diverse post-training data.
- ![2026 ICML](https://img.shields.io/badge/2026-ICML-blue) [Convex Dataset Valuation for Post-Training](https://arxiv.org/abs/2605.16704) - Dataset-level valuation and subset selection for constrained LLM post-training.
- ![2026 ICML](https://img.shields.io/badge/2026-ICML-blue) [CAReDiO: Enhancing Cultural Alignment of LLM via Representativeness and Distinctiveness Guided Data Optimization](https://icml.cc/virtual/2026/papers.html?filter=titles&search=CAReDiO%3A%20Enhancing%20Cultural%20Alignment%20of%20LLM%20via%20Representativeness%20and%20Distinctiveness%20Guided%20Data%20Optimization) - Optimizes culturally representative and distinctive alignment data.
- ![2024 arXiv](https://img.shields.io/badge/2024-arXiv-lightgrey) [LESS: Selecting Influential Data for Targeted Instruction Tuning](https://arxiv.org/abs/2402.04333) - Gradient-similarity selection for targeted skills.
- ![2024 arXiv](https://img.shields.io/badge/2024-arXiv-lightgrey) [Superfiltering: Weak-to-Strong Data Filtering for Fast Instruction-Tuning](https://arxiv.org/abs/2402.00530) - Small models filter instruction data for larger models.
- ![2024 ICLR](https://img.shields.io/badge/2024-ICLR-red) [What Makes Good Data for Alignment?](https://arxiv.org/abs/2312.15685) - Complexity, quality, diversity, and DEITA selection.
- ![2024 arXiv](https://img.shields.io/badge/2024-arXiv-lightgrey) [Magpie: Alignment Data Synthesis from Scratch by Prompting Aligned LLMs with Nothing](https://arxiv.org/abs/2406.08464) - Synthetic alignment data extraction from aligned chat templates.
- ![2023 NeurIPS](https://img.shields.io/badge/2023-NeurIPS-purple) [LIMA: Less Is More for Alignment](https://proceedings.neurips.cc/paper_files/paper/2023/hash/ac662d74829e4407ce1d126477f4a03a-Abstract-Conference.html) - Carefully curated 1K examples for supervised alignment.
- ![2023 arXiv](https://img.shields.io/badge/2023-arXiv-lightgrey) [AlpaGasus: Training A Better Alpaca with Fewer Data](https://arxiv.org/abs/2307.08701) - LLM-filtered Alpaca data.
- ![2023 arXiv](https://img.shields.io/badge/2023-arXiv-lightgrey) [Instruction Mining: Instruction Data Selection for Tuning Large Language Models](https://arxiv.org/abs/2307.06290) - Automatic instruction data selection.
- ![2023 arXiv](https://img.shields.io/badge/2023-arXiv-lightgrey) [MoDS: Model-oriented Data Selection for Instruction Tuning](https://arxiv.org/abs/2311.15653) - Quality, coverage, and necessity criteria.
- ![2023 arXiv](https://img.shields.io/badge/2023-arXiv-lightgrey) [Data Selection for Fine-tuning Large Language Models Using Transferred Shapley Values](https://arxiv.org/abs/2306.10165) - Shapley transfer for fine-tuning data.
- ![2024 ICML](https://img.shields.io/badge/2024-ICML-blue) [UltraFeedback: Boosting Language Models with Scaled AI Feedback](https://arxiv.org/abs/2310.01377) - Large-scale AI feedback preference data.
- ![2023 arXiv](https://img.shields.io/badge/2023-arXiv-lightgrey) [Orca: Progressive Learning from Complex Explanation Traces of GPT-4](https://arxiv.org/abs/2306.02707) - Explanation-trace imitation data.
- ![2023 ACL](https://img.shields.io/badge/2023-ACL-brightgreen) [Self-Instruct: Aligning Language Models with Self-Generated Instructions](https://arxiv.org/abs/2212.10560) - Pre-2023 anchor for self-generated instruction data.

## Continual Learning and Replay Data

- ![2026 ACL](https://img.shields.io/badge/2026-ACL-brightgreen) [FOREVER: Forgetting Curve-Inspired Memory Replay for Language Model Continual Learning](https://arxiv.org/abs/2601.03938) - ACL 2026; schedules replay by model-centric update time instead of fixed steps.
- ![2026 ICML](https://img.shields.io/badge/2026-ICML-blue) [Retaining by Doing: The Role of On-Policy Data in Mitigating Forgetting](https://arxiv.org/abs/2510.18874) - Shows how on-policy data reduces forgetting in post-trained language models.
- ![2025 ICML](https://img.shields.io/badge/2025-ICML-blue) [Learning Dynamics in Continual Pre-Training for Large Language Models](https://arxiv.org/abs/2505.07796) - ICML 2025 Oral; scaling law for continual pretraining with replay ratio and learning-rate effects.
- ![2025 arXiv](https://img.shields.io/badge/2025-arXiv-lightgrey) [Revisiting Replay and Gradient Alignment for Continual Pre-Training of Large Language Models](https://arxiv.org/abs/2508.01908) - Large-scale replay and meta-experience replay study for multilingual LLM continual pretraining.
- ![2024 EMNLP](https://img.shields.io/badge/2024-EMNLP-orange) [SEEKR: Selective Attention-Guided Knowledge Retention for Continual Learning of Large Language Models](https://arxiv.org/abs/2411.06171) - EMNLP 2024; attention distillation for data-efficient replay-based continual learning.
- ![2024 BMVC](https://img.shields.io/badge/2024-BMVC-blueviolet) [CLIP with Generative Latent Replay: a Strong Baseline for Incremental Learning](https://arxiv.org/abs/2407.15793) - BMVC 2024 Oral; generative latent replay for adapting CLIP while preserving zero-shot behavior.
- ![2024 NAACL](https://img.shields.io/badge/2024-NAACL-yellowgreen) [InsCL: A Data-efficient Continual Learning Paradigm for Fine-tuning Large Language Models with Instructions](https://arxiv.org/abs/2403.11435) - NAACL 2024; instruction-aware replay selection by task similarity and instruction information.
- ![2024 ACL](https://img.shields.io/badge/2024-ACL-brightgreen) [Mitigating Catastrophic Forgetting in Large Language Models with Self-Synthesized Rehearsal](https://arxiv.org/abs/2403.01244) - ACL 2024 main; synthetic rehearsal when previous training data is unavailable.
- ![2024 arXiv](https://img.shields.io/badge/2024-arXiv-lightgrey) [Simple and Scalable Strategies to Continually Pre-train Large Language Models](https://arxiv.org/abs/2403.08763) - Continual pretraining recipe combining learning-rate re-warming/re-decaying with old-data replay.

## Synthetic Data and Model Collapse

- ![2026 Dataset](https://img.shields.io/badge/2026-Dataset-yellow) [Multilingual TinyStories](https://arxiv.org/abs/2603.14563) - Synthetic Indic children's-story corpus.
- ![2026 ICML](https://img.shields.io/badge/2026-ICML-blue) [R1-SyntheticVL: Is Synthetic Data from Generative Models Ready for Multimodal Large Language Model?](https://arxiv.org/abs/2602.03300) - Collective adversarial multimodal data synthesis for MLLM training.
- ![2026 ICML](https://img.shields.io/badge/2026-ICML-blue) [Principled Synthetic Data Enables the First Scaling Laws for LLMs in Recommendation](https://arxiv.org/abs/2602.07298) - Synthetic recommendation data reveals predictable LLM scaling laws.
- ![2026 ICML](https://img.shields.io/badge/2026-ICML-blue) [PluRel: Synthetic Data unlocks Scaling Laws for Relational Foundation Models](https://arxiv.org/abs/2602.04029) - Synthetic relational data for scaling-law studies in relational foundation models.
- ![2026 ICML](https://img.shields.io/badge/2026-ICML-blue) [Privasis: Synthesizing the Largest "Public" Private Dataset from Scratch](https://arxiv.org/abs/2602.03183) - Million-scale synthetic private-information corpus for privacy research.
- ![2026 ICML](https://img.shields.io/badge/2026-ICML-blue) [Ambient Dataloops: Generative Models for Dataset Refinement](https://arxiv.org/abs/2601.15417) - Iterative dataset-model refinement without destructive self-consuming loops.
- ![2026 ICML](https://img.shields.io/badge/2026-ICML-blue) [Curated Synthetic Data Doesn't Have to Collapse: A Theoretical Study of Generative Retraining with Pluralistic Preferences](https://arxiv.org/abs/2605.07724) - Theoretical analysis of preference-curated synthetic retraining without collapse.
- ![2026 ICML](https://img.shields.io/badge/2026-ICML-blue) [Reasoning-Driven Synthetic Data Generation and Evaluation](https://arxiv.org/abs/2603.29791) - Agentic reasoning-driven mechanism for controllable synthetic dataset generation.
- ![2025 arXiv](https://img.shields.io/badge/2025-arXiv-lightgrey) [Multi-modal Synthetic Data Training and Model Collapse](https://arxiv.org/abs/2505.08803) - Model collapse in VLMs and diffusion models.
- ![2025 arXiv](https://img.shields.io/badge/2025-arXiv-lightgrey) [Escaping Model Collapse via Synthetic Data Verification](https://arxiv.org/abs/2510.16657) - Verified synthetic data and long-run convergence.
- ![2024 arXiv](https://img.shields.io/badge/2024-arXiv-lightgrey) [Is Model Collapse Inevitable?](https://arxiv.org/abs/2404.01413) - Shows accumulation of real plus synthetic data can avoid collapse.
- ![2024 arXiv](https://img.shields.io/badge/2024-arXiv-lightgrey) [Model Collapse Demystified: The Case of Regression](https://arxiv.org/abs/2402.07712) - Theoretical analysis in regression.
- ![2024 arXiv](https://img.shields.io/badge/2024-arXiv-lightgrey) [A Tale of Tails: Model Collapse as a Change of Scaling Laws](https://arxiv.org/abs/2402.07043) - Tail behavior and scaling laws under collapse.
- ![2024 arXiv](https://img.shields.io/badge/2024-arXiv-lightgrey) [How Bad is Training on Synthetic Data?](https://arxiv.org/abs/2404.05090) - Statistical analysis of language model collapse.
- ![2024 arXiv](https://img.shields.io/badge/2024-arXiv-lightgrey) [A Note on Shumailov et al. (2024)](https://arxiv.org/abs/2410.12954) - Follow-up theoretical note on recursive generation.
- ![2024 Nature](https://img.shields.io/badge/2024-Nature-success) [The Curse of Recursion: Training on Generated Data Makes Models Forget](https://arxiv.org/abs/2305.17493) - Foundational model-collapse paper.
- ![2024 ICLR](https://img.shields.io/badge/2024-ICLR-red) [Self-Consuming Generative Models Go MAD](https://arxiv.org/abs/2307.01850) - Model autophagy disorder in generative loops.
- ![2023 arXiv](https://img.shields.io/badge/2023-arXiv-lightgrey) [The Curious Decline of Linguistic Diversity](https://arxiv.org/abs/2311.09807) - Recursive synthetic text reduces linguistic diversity.
- ![2023 Dataset](https://img.shields.io/badge/2023-Dataset-yellow) [TinyStories](https://arxiv.org/abs/2305.07759) - Synthetic stories for small language models.
- ![2023 arXiv](https://img.shields.io/badge/2023-arXiv-lightgrey) [Textbooks Are All You Need](https://arxiv.org/abs/2306.11644) - phi-1 trained with textbook-quality and synthetic code data.

## Data Attribution, Valuation, and Influence

- ![2025 arXiv](https://img.shields.io/badge/2025-arXiv-lightgrey) [From Fairness to Truthfulness: Rethinking Data Valuation Design](https://arxiv.org/abs/2504.05563) - Mechanism design for truthful data markets.
- ![2025 arXiv](https://img.shields.io/badge/2025-arXiv-lightgrey) [Efficient Forward-Only Data Valuation for Pretrained LLMs and VLMs](https://arxiv.org/abs/2508.10180) - Forward-only influence estimation.
- ![2025 arXiv](https://img.shields.io/badge/2025-arXiv-lightgrey) [Lightweight Time Series Data Valuation on Time Series Foundation Models](https://arxiv.org/abs/2511.11648) - Data valuation for time-series foundation models.
- ![2026 ICML](https://img.shields.io/badge/2026-ICML-blue) [Data Provenance Auditing of Fine-Tuned Large Language Models with a Text-Preserving Technique](https://arxiv.org/abs/2510.09655) - Text-preserving watermarking for auditing fine-tuning data provenance.
- ![2026 ICML](https://img.shields.io/badge/2026-ICML-blue) [GUDA: Counterfactual Group-wise Training Data Attribution for Diffusion Models via Unlearning](https://arxiv.org/abs/2601.22651) - Group-level diffusion data attribution via unlearning counterfactuals.
- ![2026 ICML](https://img.shields.io/badge/2026-ICML-blue) [Step-resolved data attribution for looped transformers](https://arxiv.org/abs/2602.10097) - Decomposes transformer influence estimates across recurrent reasoning steps.
- ![2026 ICML](https://img.shields.io/badge/2026-ICML-blue) [Mechanistic Data Attribution: Tracing the Training Origins of Interpretable LLM Units](https://arxiv.org/abs/2601.21996) - Traces interpretable LLM units back to influential training samples.
- ![2026 ICML](https://img.shields.io/badge/2026-ICML-blue) [Is Data Shapley Not Better than Random in Data Selection? Ask NASH](https://arxiv.org/abs/2605.10684) - Re-examines Shapley-style data selection and proposes a NASH perspective.
- ![2026 ICML](https://img.shields.io/badge/2026-ICML-blue) [ExPLAIND: Unifying Model, Data, and Training Attribution to Study Model Behavior](https://arxiv.org/abs/2505.20076) - Connects model, data, and training attribution for behavior analysis.
- ![2026 ICML](https://img.shields.io/badge/2026-ICML-blue) [DataGuard: A Non-intrusive Dataset Auditing Framework via Differential Information Forensics](https://icml.cc/virtual/2026/papers.html?filter=titles&search=DataGuard%3A%20A%20Non-intrusive%20Dataset%20Auditing%20Framework%20via%20Differential%20Information%20Forensics) - Audits dataset usage through differential information forensics.
- ![2024 arXiv](https://img.shields.io/badge/2024-arXiv-lightgrey) [DemoShapley: Valuation of Demonstrations for In-Context Learning](https://arxiv.org/abs/2410.07523) - Shapley-style valuation of ICL demonstrations.
- ![2024 NeurIPS](https://img.shields.io/badge/2024-NeurIPS-purple) [Data Attribution for Text-to-Image Models by Unlearning Synthesized Images](https://arxiv.org/abs/2406.09408) - Attribution via simulated unlearning.
- ![2024 arXiv](https://img.shields.io/badge/2024-arXiv-lightgrey) [Data Attribution for Diffusion Models: Timestep-induced Bias in Influence Estimation](https://arxiv.org/abs/2401.09031) - Diffusion-TracIn and Diffusion-ReTrac.
- ![2023 arXiv](https://img.shields.io/badge/2023-arXiv-lightgrey) [TRAK: Attributing Model Behavior at Scale](https://arxiv.org/abs/2303.14186) - Scalable random-projection attribution.
- ![2024 ICLR](https://img.shields.io/badge/2024-ICLR-red) [DataInf: Efficiently Estimating Data Influence in LoRA-tuned LLMs and Diffusion Models](https://arxiv.org/abs/2310.00902) - Influence approximation for PEFT and diffusion.
- ![2023 arXiv](https://img.shields.io/badge/2023-arXiv-lightgrey) [Training Data Attribution for Diffusion Models](https://arxiv.org/abs/2306.02174) - Ensemble-based diffusion data attribution.
- ![2023 arXiv](https://img.shields.io/badge/2023-arXiv-lightgrey) [Evaluating Data Attribution for Text-to-Image Models](https://arxiv.org/abs/2306.09345) - Evaluation setup for text-to-image attribution.

## Privacy, Copyright, Consent, and Unlearning

- ![2025 Resource](https://img.shields.io/badge/2025-Resource-informational) [FlexOlmo: Open Language Models for Flexible Data Use](https://arxiv.org/abs/2507.07024) - Data owners can include/exclude experts at inference time.
- ![2026 arXiv](https://img.shields.io/badge/2026-arXiv-lightgrey) [Pretraining Data Exposure in Large Language Models](https://arxiv.org/abs/2605.26133) - Unified survey of membership inference, contamination, and security implications.
- ![2026 ICML](https://img.shields.io/badge/2026-ICML-blue) [Extracting alignment data in open models](https://arxiv.org/abs/2510.18554) - Shows that post-training alignment data can be semantically extracted from open models.
- ![2026 ICML](https://img.shields.io/badge/2026-ICML-blue) [Provable Training Data Identification for Large Language Models](https://arxiv.org/abs/2510.09717) - Provides provable tools for identifying training data in LLMs.
- ![2026 ICML](https://img.shields.io/badge/2026-ICML-blue) [Rethinking Pretraining Data Detection for LLMs: From Local to Global](https://icml.cc/virtual/2026/papers.html?filter=titles&search=Rethinking%20Pretraining%20Data%20Detection%20for%20LLMs%3A%20From%20Local%20to%20Global) - Revisits pretraining-data detection with global evidence.
- ![2026 ICML](https://img.shields.io/badge/2026-ICML-blue) [Privacy Risks of Agentic Inferential Capabilities in Data Linkage Attacks](https://icml.cc/virtual/2026/papers.html?filter=titles&search=Privacy%20Risks%20of%20Agentic%20Inferential%20Capabilities%20in%20Data%20Linkage%20Attacks) - Studies privacy risks from agentic data linkage.
- ![2026 ICML](https://img.shields.io/badge/2026-ICML-blue) [RECOVER: Reliable Detection of Unauthorized Data Usage in Text-to-Image Diffusion Models via Inversion Robustness](https://icml.cc/virtual/2026/papers.html?filter=titles&search=RECOVER%3A%20Reliable%20Detection%20of%20Unauthorized%20Data%20Usage%20in%20Text-to-Image%20Diffusion%20Models%20via%20Inversion%20Robustness) - Detects unauthorized diffusion-model training data use via inversion robustness.
- ![2026 ICML](https://img.shields.io/badge/2026-ICML-blue) [Position: The Data Provenance-Parametric Divide in Large Language Models](https://icml.cc/virtual/2026/papers.html?filter=titles&search=Position%3A%20The%20Data%20Provenance-Parametric%20Divide%20in%20Large%20Language%20Models) - Position paper on what is captured in parameters versus provenance records.
- ![2026 ICML](https://img.shields.io/badge/2026-ICML-blue) [From Prompts to Responses: Dual-Sided Data Leakage and Defense in Split Large Language Models](https://arxiv.org/abs/2606.14210) - Studies prompt- and response-side leakage in split LLM fine-tuning.
- ![2026 ICML](https://img.shields.io/badge/2026-ICML-blue) [Minim: Privacy-Aware Minimal View for Agents via Trusted Local Sanitization](https://arxiv.org/abs/2606.13949) - Sanitizes UI observations so LLM agents receive only task-relevant private context.
- ![2024 arXiv](https://img.shields.io/badge/2024-arXiv-lightgrey) [Consent in Crisis: The Rapid Decline of the AI Data Commons](https://arxiv.org/abs/2407.14933) - Longitudinal audit of web consent and robots/ToS restrictions.
- ![2024 Dataset](https://img.shields.io/badge/2024-Dataset-yellow) [MUSE: Machine Unlearning Six-Way Evaluation for Language Models](https://arxiv.org/abs/2407.06460) - Six-axis unlearning evaluation.
- ![2024 Dataset](https://img.shields.io/badge/2024-Dataset-yellow) [TOFU: A Task of Fictitious Unlearning for LLMs](https://arxiv.org/abs/2401.06121) - Synthetic benchmark for LLM unlearning.
- ![2024 ICML](https://img.shields.io/badge/2024-ICML-blue) [The WMDP Benchmark: Measuring and Reducing Malicious Use With Unlearning](https://arxiv.org/abs/2403.03218) - Hazardous-knowledge benchmark and representation unlearning.
- ![2026 ICML](https://img.shields.io/badge/2026-ICML-blue) [ForceForget: Reinforcement Concept Removal for Enhancing Safety in Text-to-Image Models](https://arxiv.org/abs/2606.14351) - Reinforcement-based concept removal for unsafe text-to-image generations.
- ![2024 ICML](https://img.shields.io/badge/2024-ICML-blue) [Copyright Traps for Large Language Models](https://arxiv.org/abs/2402.09363) - Detecting training on protected content via traps.
- ![2024 arXiv](https://img.shields.io/badge/2024-arXiv-lightgrey) [Mosaic Memory: Fuzzy Duplication in Copyright Traps for Large Language Models](https://arxiv.org/abs/2405.15523) - Fuzzy traps and memorization.
- ![2024 arXiv](https://img.shields.io/badge/2024-arXiv-lightgrey) [Fine-tuning can Help Detect Pretraining Data from Large Language Models](https://arxiv.org/abs/2410.10880) - Fine-tuned score deviation for pretraining data detection.
- ![2024 arXiv](https://img.shields.io/badge/2024-arXiv-lightgrey) [Pretraining Data Detection for Large Language Models: A Divergence-based Calibration Method](https://arxiv.org/abs/2409.14781) - Divergence-calibrated detection.
- ![2023 Dataset](https://img.shields.io/badge/2023-Dataset-yellow) [The Data Provenance Initiative: A Large Scale Audit of Dataset Licensing & Attribution in AI](https://arxiv.org/abs/2310.16787) - Dataset license/provenance audit.
- ![2024 ICLR](https://img.shields.io/badge/2024-ICLR-red) [SILO Language Models: Isolating Legal Risk In a Nonparametric Datastore](https://arxiv.org/abs/2308.04430) - Legal-risk isolation via datastore.
- ![2023 arXiv](https://img.shields.io/badge/2023-arXiv-lightgrey) [Detecting Pretraining Data from Large Language Models](https://arxiv.org/abs/2310.16789) - Min-K% Prob and WIKIMIA.
- ![2023 arXiv](https://img.shields.io/badge/2023-arXiv-lightgrey) [Scalable Extraction of Training Data from (Production) Language Models](https://arxiv.org/abs/2311.17035) - Practical extraction from open and production LMs.
- ![2023 arXiv](https://img.shields.io/badge/2023-arXiv-lightgrey) [Large Language Model Unlearning](https://arxiv.org/abs/2310.10683) - Early formulation of LLM unlearning.

## Benchmark Contamination, Freshness, and RAG Evaluation

- ![2025 Survey](https://img.shields.io/badge/2025-Survey-9cf) [A Survey on Data Contamination for Large Language Models](https://arxiv.org/abs/2502.14425) - Contamination detection and prevention survey.
- ![2025 arXiv](https://img.shields.io/badge/2025-arXiv-lightgrey) [Signal and Noise: A Framework for Reducing Uncertainty in Language Model Evaluation](https://arxiv.org/abs/2508.13144) - Benchmark reliability for scaling decisions.
- ![2026 ICML](https://img.shields.io/badge/2026-ICML-blue) [MultiHal: Multilingual Dataset for Knowledge-Graph Grounded Evaluation of LLM Hallucinations](https://arxiv.org/abs/2505.14101) - Multilingual KG-grounded hallucination benchmark for LLM factuality.
- ![2026 ICML](https://img.shields.io/badge/2026-ICML-blue) [DSGym: A Holistic Framework for Evaluating and Training Data Science Agents](https://arxiv.org/abs/2601.16344) - Execution-grounded benchmark and training environment for data science agents.
- ![2026 ICML](https://img.shields.io/badge/2026-ICML-blue) [DeepAnalyze: Agentic Large Language Models for Autonomous Data Science](https://arxiv.org/abs/2510.16872) - Agentic LLM and data-grounded training pipeline for autonomous data science.
- ![2026 ICML](https://img.shields.io/badge/2026-ICML-blue) [Hunt Instead of Wait: Evaluating Deep Data Research on Large Language Models](https://arxiv.org/abs/2602.02039) - Open-ended benchmark for LLMs to autonomously extract insights from databases.
- ![2026 ICML](https://img.shields.io/badge/2026-ICML-blue) [CODA-BENCH: Can Code Agents Handle Data-Intensive Tasks?](https://arxiv.org/abs/2606.15300) - Benchmark for code agents operating over large-scale data and file-system tasks.
- ![2026 ICML](https://img.shields.io/badge/2026-ICML-blue) [Reward Hacking Benchmark: Measuring Exploits in LLM Agents with Tool Use](https://arxiv.org/abs/2605.02964) - Multi-step tool-use benchmark for reward hacking and shortcut exploitation.
- ![2026 ICML](https://img.shields.io/badge/2026-ICML-blue) [A Benchmark and Framework for Evaluating Next Action Predictions in Spreadsheets](https://arxiv.org/abs/2606.13802) - Spreadsheet next-action prediction benchmark for structured-data workflows.
- ![2026 ICML](https://img.shields.io/badge/2026-ICML-blue) [Temporal Preference Optimization for Unsupervised Retrieval](https://arxiv.org/abs/2606.17664) - Optimizes dense retrievers for temporal relevance without labeled supervision.
- ![2024 Dataset](https://img.shields.io/badge/2024-Dataset-yellow) [LiveBench: A Challenging, Contamination-Free LLM Benchmark](https://arxiv.org/abs/2406.19314) - Frequently updated benchmark with objective ground truth.
- ![2024 Dataset](https://img.shields.io/badge/2024-Dataset-yellow) [CRUD-RAG](https://arxiv.org/abs/2401.17043) - RAG benchmark across create/read/update/delete scenarios.
- ![2024 Dataset](https://img.shields.io/badge/2024-Dataset-yellow) [RAGTruth](https://arxiv.org/abs/2401.00396) - Word-level hallucination corpus for RAG systems.
- ![2023 arXiv](https://img.shields.io/badge/2023-arXiv-lightgrey) [Rethinking Benchmark and Contamination for Language Models with Rephrased Samples](https://arxiv.org/abs/2311.04850) - Rephrased contamination and stronger decontamination.
- ![2023 Resource](https://img.shields.io/badge/2023-Resource-informational) [FreshLLMs](https://arxiv.org/abs/2310.03214) - FreshQA and search-augmented prompting for changing knowledge.
- ![2024 NAACL](https://img.shields.io/badge/2024-NAACL-yellowgreen) [ARES: An Automated Evaluation Framework for Retrieval-Augmented Generation Systems](https://arxiv.org/abs/2311.09476) - Synthetic judges plus small human sets for RAG evaluation.
- ![2023 Resource](https://img.shields.io/badge/2023-Resource-informational) [Self-RAG: Learning to Retrieve, Generate, and Critique through Self-Reflection](https://arxiv.org/abs/2310.11511) - Trains models to decide when and how to retrieve.

## Multimodal and Vision-Language Data

- ![2025 arXiv](https://img.shields.io/badge/2025-arXiv-lightgrey) [Multi-modal Synthetic Data Training and Model Collapse](https://arxiv.org/abs/2505.08803) - Synthetic feedback loops in multimodal systems.
- ![2025 Dataset](https://img.shields.io/badge/2025-Dataset-yellow) [Safe RLHF-V](https://arxiv.org/abs/2503.17682) - Multimodal helpfulness/safety preference data.
- ![2026 ICML](https://img.shields.io/badge/2026-ICML-blue) [Data Selection for Fine-tuning Vision Language Models via Cross Modal Alignment Trajectories](https://arxiv.org/abs/2510.01454) - Data-efficient LVLM instruction tuning via cross-modal attention trajectories.
- ![2026 ICML](https://img.shields.io/badge/2026-ICML-blue) [OpenGPT-4o-Image: A Comprehensive Dataset for Advanced Image Generation and Editing](https://arxiv.org/abs/2509.24900) - Hierarchical instruction-image dataset for advanced image generation/editing.
- ![2026 ICML](https://img.shields.io/badge/2026-ICML-blue) [TextAtlas5M: A Large-scale Dataset for Dense Text Image Generation](https://arxiv.org/abs/2502.07870) - Large-scale dataset and benchmark for long-text image generation.
- ![2024 arXiv](https://img.shields.io/badge/2024-arXiv-lightgrey) [Cambrian-1: A Fully Open, Vision-Centric Exploration of Multimodal LLMs](https://arxiv.org/abs/2406.16860) - Open cookbook with visual data mixture analysis.
- ![2024 Dataset](https://img.shields.io/badge/2024-Dataset-yellow) [DataComp-LM](https://arxiv.org/abs/2406.11794) - LM counterpart to DataComp, useful for multimodal-data methodology comparisons.
- ![2024 NeurIPS](https://img.shields.io/badge/2024-NeurIPS-purple) [Data Attribution for Text-to-Image Models by Unlearning Synthesized Images](https://arxiv.org/abs/2406.09408) - Multimodal provenance/attribution.
- ![2024 arXiv](https://img.shields.io/badge/2024-arXiv-lightgrey) [Data Attribution for Diffusion Models: Timestep-induced Bias in Influence Estimation](https://arxiv.org/abs/2401.09031) - Influence estimation for diffusion timesteps.
- ![2023 Dataset](https://img.shields.io/badge/2023-Dataset-yellow) [DataComp: In search of the next generation of multimodal datasets](https://arxiv.org/abs/2304.14108) - Benchmark for image-text dataset design.
- ![2023 Dataset](https://img.shields.io/badge/2023-Dataset-yellow) [ShareGPT4V: Improving Large Multi-Modal Models with Better Captions](https://arxiv.org/abs/2311.12793) - High-quality detailed caption data.
- ![2023 arXiv](https://img.shields.io/badge/2023-arXiv-lightgrey) [Visual Instruction Tuning](https://arxiv.org/abs/2304.08485) - LLaVA synthetic multimodal instruction data.
- ![2023 arXiv](https://img.shields.io/badge/2023-arXiv-lightgrey) [Training Data Attribution for Diffusion Models](https://arxiv.org/abs/2306.02174) - Attribution for diffusion outputs.

## Safety, Fairness, and Data Poisoning

- ![2026 arXiv](https://img.shields.io/badge/2026-arXiv-lightgrey) [Loss Landscape Poisoning: Targeted Extraction of Unseen Training Data from LLMs](https://arxiv.org/abs/2606.17110) - Poisoning to amplify privacy leakage.
- ![2026 ICML](https://img.shields.io/badge/2026-ICML-blue) [Rapid Poison: Practical Poisoning Attacks Against the Rapid Response Framework](https://arxiv.org/abs/2606.16242) - Practical poisoning attack against continuously updated jailbreak-detection classifiers.
- ![2026 ICML](https://img.shields.io/badge/2026-ICML-blue) [Detecting and Filtering Unsafe Training Data via Data Attribution](https://arxiv.org/abs/2502.11411) - Uses data attribution to identify and filter unsafe LLM training examples.
- ![2025 Dataset](https://img.shields.io/badge/2025-Dataset-yellow) [Safe RLHF-V](https://arxiv.org/abs/2503.17682) - Safety alignment data for MLLMs.
- ![2024 Dataset](https://img.shields.io/badge/2024-Dataset-yellow) [PKU-SafeRLHF](https://arxiv.org/abs/2406.15513) - Multi-level safety preference data.
- ![2024 Dataset](https://img.shields.io/badge/2024-Dataset-yellow) [A Chinese Dataset for Evaluating the Safeguards in Large Language Models](https://arxiv.org/abs/2402.12193) - Chinese safeguard evaluation data.
- ![2024 arXiv](https://img.shields.io/badge/2024-arXiv-lightgrey) [Sleeper Agents: Training Deceptive LLMs that Persist Through Safety Training](https://arxiv.org/abs/2401.05566) - Backdoor behavior induced during training.
- ![2023 Dataset](https://img.shields.io/badge/2023-Dataset-yellow) [BeaverTails](https://arxiv.org/abs/2307.04657) - Helpfulness/harmlessness preference and safety labels.
- ![2023 Dataset](https://img.shields.io/badge/2023-Dataset-yellow) [Do-Not-Answer](https://arxiv.org/abs/2308.13387) - Dataset of instructions responsible models should refuse.
- ![2023 Resource](https://img.shields.io/badge/2023-Resource-informational) [DecodingTrust](https://arxiv.org/abs/2306.11698) - Trustworthiness benchmark spanning toxicity, bias, privacy, and robustness.
- ![2023 Dataset](https://img.shields.io/badge/2023-Dataset-yellow) [Poisoning Web-Scale Training Datasets is Practical](https://arxiv.org/abs/2302.10149) - Split-view and frontrunning poisoning of web-scale datasets.
- ![2023 arXiv](https://img.shields.io/badge/2023-arXiv-lightgrey) [Poisoning Language Models During Instruction Tuning](https://arxiv.org/abs/2305.00944) - Poison examples in instruction data.

## Classic References

These are older than the main 2023+ window but useful for context.

- ![2022 arXiv](https://img.shields.io/badge/2022-arXiv-lightgrey) [Can Foundation Models Wrangle Your Data?](https://arxiv.org/abs/2205.09911) - Foundation models for classical data cleaning and integration.
- ![2023 ACL](https://img.shields.io/badge/2023-ACL-brightgreen) [Self-Instruct](https://arxiv.org/abs/2212.10560) - Synthetic instruction bootstrapping.
- ![2021 arXiv](https://img.shields.io/badge/2021-arXiv-lightgrey) [On the Opportunities and Risks of Foundation Models](https://arxiv.org/abs/2108.07258) - Broad foundation model framing.
- ![2021 USENIX](https://img.shields.io/badge/2021-USENIX-lightgrey) [Extracting Training Data from Large Language Models](https://www.usenix.org/conference/usenixsecurity21/presentation/carlini-extracting) - Early memorization and extraction study.

## Related Workshops and Resources

- [DATA-FM @ ICLR 2025](https://datafm.github.io/) - 2nd Workshop on Navigating and Addressing Data Problems for Foundation Models.
- [DPFM @ ICLR 2024](https://sites.google.com/view/dpfm-iclr24/home) - First workshop on Data Problems for Foundation Models.
- [ICLR 2025 DATA-FM OpenReview](https://openreview.net/group?id=ICLR.cc/2025/Workshop/Data_Problems) - Accepted workshop submissions.
- [Data Provenance Explorer](https://www.dataprovenance.org/) - Dataset licensing and attribution explorer.
- [DataComp](https://www.datacomp.ai/) - Multimodal data curation benchmark.
- [DCLM / DataComp-LM](https://www.datacomp.ai/dclm/) - Language-model dataset benchmark.
- [Dolma Toolkit](https://github.com/allenai/dolma) - Open data curation toolkit.
- [FineWeb](https://huggingface.co/datasets/HuggingFaceFW/fineweb) - Hugging Face FineWeb dataset page.

## Contributing

Pull requests are welcome. Please prefer papers that have a clear data-centric contribution, include a stable paper link, and add the paper to both the README and `data/papers.yaml` when possible.
