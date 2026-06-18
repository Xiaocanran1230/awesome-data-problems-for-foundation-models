# Awesome Data Problems for Foundation Models

> A curated reading list on data problems for foundation models, inspired by the DATA-FM / DPFM workshops and Awesome-style paper repositories.

Foundation models are increasingly limited, shaped, and governed by their data: how it is collected, filtered, mixed, valued, attributed, protected, evaluated, and regenerated. This repository tracks recent papers, datasets, benchmarks, and position work on **data-centric foundation model research**, with an emphasis on work from 2023 onward.

## Scope

The taxonomy follows the DATA-FM workshop themes: data collection and curation, data attribution and valuation, legal/copyright and privacy, synthetic data and model collapse, safety/fairness, and benchmark contamination/evaluation. Borderline papers are included when their main contribution changes how data is sourced, selected, audited, or evaluated for foundation models.

## Contents

- [Surveys and Position Papers](#surveys-and-position-papers)
- [Open Corpora, Recipes, and Data-Centric Model Releases](#open-corpora-recipes-and-data-centric-model-releases)
- [Pretraining Data Selection, Filtering, and Mixing](#pretraining-data-selection-filtering-and-mixing)
- [Instruction, Preference, and Alignment Data](#instruction-preference-and-alignment-data)
- [Synthetic Data and Model Collapse](#synthetic-data-and-model-collapse)
- [Data Attribution, Valuation, and Influence](#data-attribution-valuation-and-influence)
- [Privacy, Copyright, Consent, and Unlearning](#privacy-copyright-consent-and-unlearning)
- [Benchmark Contamination, Freshness, and RAG Evaluation](#benchmark-contamination-freshness-and-rag-evaluation)
- [Multimodal and Vision-Language Data](#multimodal-and-vision-language-data)
- [Safety, Fairness, and Data Poisoning](#safety-fairness-and-data-poisoning)
- [Classic References](#classic-references)
- [Related Workshops and Resources](#related-workshops-and-resources)

## Surveys and Position Papers

- [2025] [Rethinking Data Mixture for Large Language Models: A Comprehensive Survey and New Perspectives](https://arxiv.org/abs/2505.21598) - Survey of offline/online data mixture optimization.
- [2025] [A Survey on Data Contamination for Large Language Models](https://arxiv.org/abs/2502.14425) - Survey of contamination-free evaluation and contamination detection.
- [2025] [A Survey on Efficient Large Language Model Training: From Data-centric Perspectives](https://arxiv.org/abs/2510.25817) - Data-efficient post-training taxonomy.
- [2025] [Ten Challenging Problems in Federated Foundation Models](https://arxiv.org/abs/2502.12176) - Includes private data, heterogeneity, unlearning, incentives, and privacy in FedFMs.
- [2024] [A Survey on Data Selection for Language Models](https://arxiv.org/abs/2402.16827) - Broad taxonomy of LM data selection methods.
- [2024] [A Survey on Data Synthesis and Augmentation for Large Language Models](https://arxiv.org/abs/2410.12896) - Data synthesis across pretraining, instruction tuning, and preference learning.
- [2024] [Data-Centric Foundation Models in Computational Healthcare: A Survey](https://arxiv.org/abs/2401.02458) - Healthcare-specific data quality, privacy, annotation, and ethics.
- [2024] [Benchmark Data Contamination of Large Language Models: A Survey](https://arxiv.org/abs/2406.04244) - Benchmark contamination risks and mitigations.
- [2023] [Data-centric Artificial Intelligence: A Survey](https://arxiv.org/abs/2303.10158) - General data-centric AI lifecycle survey.

## Open Corpora, Recipes, and Data-Centric Model Releases

- [2026] [How2Everything: Mining the Web for How-To Procedures to Evaluate and Improve LLMs](https://arxiv.org/abs/2602.08808) - Web-mined procedural data, benchmark, scoring, and RL loop.
- [2025] [The Common Pile v0.1: An 8TB Dataset of Public Domain and Openly Licensed Text](https://arxiv.org/abs/2506.05209) - Public-domain/openly licensed pretraining corpus and Comma models.
- [2025] [FlexOlmo: Open Language Models for Flexible Data Use](https://arxiv.org/abs/2507.07024) - Modular data ownership and inference-time inclusion/exclusion of data experts.
- [2025] [2 OLMo 2 Furious](https://arxiv.org/abs/2501.00656) - Fully open OLMo 2 recipes, staged data mixtures, and instruction data.
- [2024] [OLMo: Accelerating the Science of Language Models](https://arxiv.org/abs/2402.00838) - Open model release with training data, logs, code, and checkpoints.
- [2024] [Dolma: an Open Corpus of Three Trillion Tokens for Language Model Pretraining Research](https://arxiv.org/abs/2402.00159) - Open corpus and curation toolkit.
- [2024] [The FineWeb Datasets: Decanting the Web for the Finest Text Data at Scale](https://arxiv.org/abs/2406.17557) - 15T-token web corpus plus filtering/deduplication ablations.
- [2024] [DataComp-LM: In search of the next generation of training sets for language models](https://arxiv.org/abs/2406.11794) - Standardized benchmark for LM dataset experiments.
- [2023] [CulturaX: A Cleaned, Enormous, and Multilingual Dataset for Large Language Models in 167 Languages](https://arxiv.org/abs/2309.09400) - Multilingual cleaned and deduplicated corpus.
- [2023] [The RefinedWeb Dataset for Falcon LLM](https://arxiv.org/abs/2306.01116) - Web-only filtered/deduplicated corpus for Falcon.
- [2023] [DataComp: In search of the next generation of multimodal datasets](https://arxiv.org/abs/2304.14108) - Multimodal data curation benchmark for CLIP-style training.

## Pretraining Data Selection, Filtering, and Mixing

- [2025] [Organize the Web: Constructing Domains Enhances Pre-Training Data Curation](https://arxiv.org/abs/2502.10341) - Topic/format domain construction for web corpora.
- [2025] [Data Mixing Can Induce Phase Transitions in Knowledge Acquisition](https://openreview.net/forum?id=ZKA4yiGdrA) - DATA-FM 2025 oral on knowledge-dense mixtures and thresholds.
- [2025] [MASS: Mathematical Data Selection via Skill Graphs for Pretraining Large Language Models](https://arxiv.org/abs/2503.14917) - Skill-graph-based mathematical data selection.
- [2025] [TiKMiX: Take Data Influence into Dynamic Mixture for Language Model Pre-training](https://arxiv.org/abs/2508.17677) - Dynamic mixture optimization via group influence.
- [2024] [Data Mixing Laws: Optimizing Data Mixtures by Predicting Language Modeling Performance](https://arxiv.org/abs/2403.16952) - Predicting performance from mixture proportions.
- [2024] [RegMix: Data Mixture as Regression for Language Model Pre-training](https://arxiv.org/abs/2407.01492) - Predicts good mixtures using many small proxy trainings.
- [2024] [QuRating: Selecting High-Quality Data for Training Language Models](https://arxiv.org/abs/2402.09739) - LLM-derived quality ratings for pretraining data.
- [2024] [Rho-1: Not All Tokens Are What You Need](https://arxiv.org/abs/2404.07965) - Selective language modeling at token level.
- [2024] [Data Engineering for Scaling Language Models to 128K Context](https://arxiv.org/abs/2402.10171) - Long-context continual pretraining data recipe.
- [2024] [Data Proportion Detection for Optimized Data Management for Large Language Models](https://arxiv.org/abs/2409.17527) - Inferring pretraining data proportions from outputs.
- [2024] [Rephrasing natural text data with different languages and quality levels for Large Language Model pre-training](https://arxiv.org/abs/2410.20796) - Rephrasing natural text as pretraining augmentation.
- [2023] [DoReMi: Optimizing Data Mixtures Speeds Up Language Model Pretraining](https://arxiv.org/abs/2305.10429) - Domain reweighting with minimax optimization.
- [2023] [Data Selection for Language Models via Importance Resampling](https://arxiv.org/abs/2302.03169) - DSIR data selection using target distribution matching.
- [2023] [Skill-it! A Data-Driven Skills Framework for Understanding and Training Language Models](https://arxiv.org/abs/2307.14430) - Skill-aware online sampling and curriculum.

## Instruction, Preference, and Alignment Data

- [2026] [How2Everything: Mining the Web for How-To Procedures to Evaluate and Improve LLMs](https://arxiv.org/abs/2602.08808) - Also relevant as procedural instruction data.
- [2024] [LESS: Selecting Influential Data for Targeted Instruction Tuning](https://arxiv.org/abs/2402.04333) - Gradient-similarity selection for targeted skills.
- [2024] [Superfiltering: Weak-to-Strong Data Filtering for Fast Instruction-Tuning](https://arxiv.org/abs/2402.00530) - Small models filter instruction data for larger models.
- [2024] [What Makes Good Data for Alignment?](https://arxiv.org/abs/2312.15685) - Complexity, quality, diversity, and DEITA selection.
- [2024] [Magpie: Alignment Data Synthesis from Scratch by Prompting Aligned LLMs with Nothing](https://arxiv.org/abs/2406.08464) - Synthetic alignment data extraction from aligned chat templates.
- [2023] [LIMA: Less Is More for Alignment](https://arxiv.org/abs/2305.11206) - Carefully curated 1K examples for supervised alignment.
- [2023] [AlpaGasus: Training A Better Alpaca with Fewer Data](https://arxiv.org/abs/2307.08701) - LLM-filtered Alpaca data.
- [2023] [Instruction Mining: Instruction Data Selection for Tuning Large Language Models](https://arxiv.org/abs/2307.06290) - Automatic instruction data selection.
- [2023] [MoDS: Model-oriented Data Selection for Instruction Tuning](https://arxiv.org/abs/2311.15653) - Quality, coverage, and necessity criteria.
- [2023] [Data Selection for Fine-tuning Large Language Models Using Transferred Shapley Values](https://arxiv.org/abs/2306.10165) - Shapley transfer for fine-tuning data.
- [2023] [UltraFeedback: Boosting Language Models with Scaled AI Feedback](https://arxiv.org/abs/2310.01377) - Large-scale AI feedback preference data.
- [2023] [Orca: Progressive Learning from Complex Explanation Traces of GPT-4](https://arxiv.org/abs/2306.02707) - Explanation-trace imitation data.
- [2022] [Self-Instruct: Aligning Language Models with Self-Generated Instructions](https://arxiv.org/abs/2212.10560) - Pre-2023 anchor for self-generated instruction data.

## Synthetic Data and Model Collapse

- [2026] [Multilingual TinyStories](https://arxiv.org/abs/2603.14563) - Synthetic Indic children's-story corpus.
- [2025] [Multi-modal Synthetic Data Training and Model Collapse](https://arxiv.org/abs/2505.08803) - Model collapse in VLMs and diffusion models.
- [2025] [Escaping Model Collapse via Synthetic Data Verification](https://arxiv.org/abs/2510.16657) - Verified synthetic data and long-run convergence.
- [2024] [Is Model Collapse Inevitable?](https://arxiv.org/abs/2404.01413) - Shows accumulation of real plus synthetic data can avoid collapse.
- [2024] [Model Collapse Demystified: The Case of Regression](https://arxiv.org/abs/2402.07712) - Theoretical analysis in regression.
- [2024] [A Tale of Tails: Model Collapse as a Change of Scaling Laws](https://arxiv.org/abs/2402.07043) - Tail behavior and scaling laws under collapse.
- [2024] [How Bad is Training on Synthetic Data?](https://arxiv.org/abs/2404.05090) - Statistical analysis of language model collapse.
- [2024] [A Note on Shumailov et al. (2024)](https://arxiv.org/abs/2410.12954) - Follow-up theoretical note on recursive generation.
- [2023] [The Curse of Recursion: Training on Generated Data Makes Models Forget](https://arxiv.org/abs/2305.17493) - Foundational model-collapse paper.
- [2023] [Self-Consuming Generative Models Go MAD](https://arxiv.org/abs/2307.01850) - Model autophagy disorder in generative loops.
- [2023] [The Curious Decline of Linguistic Diversity](https://arxiv.org/abs/2311.09807) - Recursive synthetic text reduces linguistic diversity.
- [2023] [TinyStories](https://arxiv.org/abs/2305.07759) - Synthetic stories for small language models.
- [2023] [Textbooks Are All You Need](https://arxiv.org/abs/2306.11644) - phi-1 trained with textbook-quality and synthetic code data.

## Data Attribution, Valuation, and Influence

- [2025] [From Fairness to Truthfulness: Rethinking Data Valuation Design](https://arxiv.org/abs/2504.05563) - Mechanism design for truthful data markets.
- [2025] [Efficient Forward-Only Data Valuation for Pretrained LLMs and VLMs](https://arxiv.org/abs/2508.10180) - Forward-only influence estimation.
- [2025] [Lightweight Time Series Data Valuation on Time Series Foundation Models](https://arxiv.org/abs/2511.11648) - Data valuation for time-series foundation models.
- [2024] [DemoShapley: Valuation of Demonstrations for In-Context Learning](https://arxiv.org/abs/2410.07523) - Shapley-style valuation of ICL demonstrations.
- [2024] [Data Attribution for Text-to-Image Models by Unlearning Synthesized Images](https://arxiv.org/abs/2406.09408) - Attribution via simulated unlearning.
- [2024] [Data Attribution for Diffusion Models: Timestep-induced Bias in Influence Estimation](https://arxiv.org/abs/2401.09031) - Diffusion-TracIn and Diffusion-ReTrac.
- [2023] [TRAK: Attributing Model Behavior at Scale](https://arxiv.org/abs/2303.14186) - Scalable random-projection attribution.
- [2023] [DataInf: Efficiently Estimating Data Influence in LoRA-tuned LLMs and Diffusion Models](https://arxiv.org/abs/2310.00902) - Influence approximation for PEFT and diffusion.
- [2023] [Training Data Attribution for Diffusion Models](https://arxiv.org/abs/2306.02174) - Ensemble-based diffusion data attribution.
- [2023] [Evaluating Data Attribution for Text-to-Image Models](https://arxiv.org/abs/2306.09345) - Evaluation setup for text-to-image attribution.

## Privacy, Copyright, Consent, and Unlearning

- [2025] [FlexOlmo: Open Language Models for Flexible Data Use](https://arxiv.org/abs/2507.07024) - Data owners can include/exclude experts at inference time.
- [2026] [Pretraining Data Exposure in Large Language Models](https://arxiv.org/abs/2605.26133) - Unified survey of membership inference, contamination, and security implications.
- [2024] [Consent in Crisis: The Rapid Decline of the AI Data Commons](https://arxiv.org/abs/2407.14933) - Longitudinal audit of web consent and robots/ToS restrictions.
- [2024] [MUSE: Machine Unlearning Six-Way Evaluation for Language Models](https://arxiv.org/abs/2407.06460) - Six-axis unlearning evaluation.
- [2024] [TOFU: A Task of Fictitious Unlearning for LLMs](https://arxiv.org/abs/2401.06121) - Synthetic benchmark for LLM unlearning.
- [2024] [The WMDP Benchmark: Measuring and Reducing Malicious Use With Unlearning](https://arxiv.org/abs/2403.03218) - Hazardous-knowledge benchmark and representation unlearning.
- [2024] [Copyright Traps for Large Language Models](https://arxiv.org/abs/2402.09363) - Detecting training on protected content via traps.
- [2024] [Mosaic Memory: Fuzzy Duplication in Copyright Traps for Large Language Models](https://arxiv.org/abs/2405.15523) - Fuzzy traps and memorization.
- [2024] [Fine-tuning can Help Detect Pretraining Data from Large Language Models](https://arxiv.org/abs/2410.10880) - Fine-tuned score deviation for pretraining data detection.
- [2024] [Pretraining Data Detection for Large Language Models: A Divergence-based Calibration Method](https://arxiv.org/abs/2409.14781) - Divergence-calibrated detection.
- [2023] [The Data Provenance Initiative: A Large Scale Audit of Dataset Licensing & Attribution in AI](https://arxiv.org/abs/2310.16787) - Dataset license/provenance audit.
- [2023] [SILO Language Models: Isolating Legal Risk In a Nonparametric Datastore](https://arxiv.org/abs/2308.04430) - Legal-risk isolation via datastore.
- [2023] [Detecting Pretraining Data from Large Language Models](https://arxiv.org/abs/2310.16789) - Min-K% Prob and WIKIMIA.
- [2023] [Scalable Extraction of Training Data from (Production) Language Models](https://arxiv.org/abs/2311.17035) - Practical extraction from open and production LMs.
- [2023] [Large Language Model Unlearning](https://arxiv.org/abs/2310.10683) - Early formulation of LLM unlearning.

## Benchmark Contamination, Freshness, and RAG Evaluation

- [2025] [A Survey on Data Contamination for Large Language Models](https://arxiv.org/abs/2502.14425) - Contamination detection and prevention survey.
- [2025] [Signal and Noise: A Framework for Reducing Uncertainty in Language Model Evaluation](https://arxiv.org/abs/2508.13144) - Benchmark reliability for scaling decisions.
- [2024] [LiveBench: A Challenging, Contamination-Free LLM Benchmark](https://arxiv.org/abs/2406.19314) - Frequently updated benchmark with objective ground truth.
- [2024] [CRUD-RAG](https://arxiv.org/abs/2401.17043) - RAG benchmark across create/read/update/delete scenarios.
- [2024] [RAGTruth](https://arxiv.org/abs/2401.00396) - Word-level hallucination corpus for RAG systems.
- [2023] [Rethinking Benchmark and Contamination for Language Models with Rephrased Samples](https://arxiv.org/abs/2311.04850) - Rephrased contamination and stronger decontamination.
- [2023] [FreshLLMs](https://arxiv.org/abs/2310.03214) - FreshQA and search-augmented prompting for changing knowledge.
- [2023] [ARES: An Automated Evaluation Framework for Retrieval-Augmented Generation Systems](https://arxiv.org/abs/2311.09476) - Synthetic judges plus small human sets for RAG evaluation.
- [2023] [Self-RAG: Learning to Retrieve, Generate, and Critique through Self-Reflection](https://arxiv.org/abs/2310.11511) - Trains models to decide when and how to retrieve.

## Multimodal and Vision-Language Data

- [2025] [Multi-modal Synthetic Data Training and Model Collapse](https://arxiv.org/abs/2505.08803) - Synthetic feedback loops in multimodal systems.
- [2025] [Safe RLHF-V](https://arxiv.org/abs/2503.17682) - Multimodal helpfulness/safety preference data.
- [2024] [Cambrian-1: A Fully Open, Vision-Centric Exploration of Multimodal LLMs](https://arxiv.org/abs/2406.16860) - Open cookbook with visual data mixture analysis.
- [2024] [DataComp-LM](https://arxiv.org/abs/2406.11794) - LM counterpart to DataComp, useful for multimodal-data methodology comparisons.
- [2024] [Data Attribution for Text-to-Image Models by Unlearning Synthesized Images](https://arxiv.org/abs/2406.09408) - Multimodal provenance/attribution.
- [2024] [Data Attribution for Diffusion Models: Timestep-induced Bias in Influence Estimation](https://arxiv.org/abs/2401.09031) - Influence estimation for diffusion timesteps.
- [2023] [DataComp: In search of the next generation of multimodal datasets](https://arxiv.org/abs/2304.14108) - Benchmark for image-text dataset design.
- [2023] [ShareGPT4V: Improving Large Multi-Modal Models with Better Captions](https://arxiv.org/abs/2311.12793) - High-quality detailed caption data.
- [2023] [Visual Instruction Tuning](https://arxiv.org/abs/2304.08485) - LLaVA synthetic multimodal instruction data.
- [2023] [Training Data Attribution for Diffusion Models](https://arxiv.org/abs/2306.02174) - Attribution for diffusion outputs.

## Safety, Fairness, and Data Poisoning

- [2026] [Loss Landscape Poisoning: Targeted Extraction of Unseen Training Data from LLMs](https://arxiv.org/abs/2606.17110) - Poisoning to amplify privacy leakage.
- [2025] [Safe RLHF-V](https://arxiv.org/abs/2503.17682) - Safety alignment data for MLLMs.
- [2024] [PKU-SafeRLHF](https://arxiv.org/abs/2406.15513) - Multi-level safety preference data.
- [2024] [A Chinese Dataset for Evaluating the Safeguards in Large Language Models](https://arxiv.org/abs/2402.12193) - Chinese safeguard evaluation data.
- [2024] [Sleeper Agents: Training Deceptive LLMs that Persist Through Safety Training](https://arxiv.org/abs/2401.05566) - Backdoor behavior induced during training.
- [2023] [BeaverTails](https://arxiv.org/abs/2307.04657) - Helpfulness/harmlessness preference and safety labels.
- [2023] [Do-Not-Answer](https://arxiv.org/abs/2308.13387) - Dataset of instructions responsible models should refuse.
- [2023] [DecodingTrust](https://arxiv.org/abs/2306.11698) - Trustworthiness benchmark spanning toxicity, bias, privacy, and robustness.
- [2023] [Poisoning Web-Scale Training Datasets is Practical](https://arxiv.org/abs/2302.10149) - Split-view and frontrunning poisoning of web-scale datasets.
- [2023] [Poisoning Language Models During Instruction Tuning](https://arxiv.org/abs/2305.00944) - Poison examples in instruction data.

## Classic References

These are older than the main 2023+ window but useful for context.

- [2022] [Can Foundation Models Wrangle Your Data?](https://arxiv.org/abs/2205.09911) - Foundation models for classical data cleaning and integration.
- [2022] [Self-Instruct](https://arxiv.org/abs/2212.10560) - Synthetic instruction bootstrapping.
- [2021] [On the Opportunities and Risks of Foundation Models](https://arxiv.org/abs/2108.07258) - Broad foundation model framing.
- [2021] [Extracting Training Data from Large Language Models](https://www.usenix.org/conference/usenixsecurity21/presentation/carlini-extracting) - Early memorization and extraction study.

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
