# AI Papers of The Week

As a researcher, I frequently read AI papers and am trying to create this repository to record some highlighted AI papers that I read each week.

Here is the weekly series:

## 2024

- [AI Papers of the Week (April 29 - May 5)](./#ai-papers-of-the-week-april-29---may-5---2024)
- [AI Papers of the Week (April 22 - April 28)](./#ai-papers-of-the-week-april-22---april-28---2024)
- [AI Papers of the Week (April 15 - April 21)](./#ai-papers-of-the-week-april-15---april-21---2024)


## AI Papers of the Week (April 29 - May 5) - 2024
| **Paper**  | **Release Date** | **Links** |
| ------------- | ------------- | ------------- |
| (1) **AdvPrompter: Fast Adaptive Adversarial Prompting for LLMs** - The paper introduces AdvPrompter, a method to rapidly generate human-readable adversarial prompts to expose vulnerabilities in Large Language Models (LLMs). This approach, which is about 800 times faster than previous methods, does not require gradient information from the target LLM. It involves a two-step training process using high-quality adversarial suffixes and low-rank fine-tuning. The trained AdvPrompter is effective in deceiving LLMs into producing harmful responses, improving the robustness of LLMs against adversarial attacks. | April 21, 2024 | [Paper](https://arxiv.org/abs/2404.16873)|
| (2) **Replacing Judges with Juries: Evaluating LLM Generations with a Panel of Diverse Models** - The paper proposes using a panel of smaller language models (PoLL) to evaluate the output of large language models (LLMs) instead of a single large model. This approach aims to reduce cost and bias while improving evaluation accuracy. The authors demonstrate that a diverse panel of models provides better, less biased assessments and is more cost-effective than using a single large model for evaluating LLMs.  | April 29, 2024 | [Paper](https://arxiv.org/abs/2404.18796)|
| (3) **Extending Llama-3’s Context Ten-Fold Overnight** - The study extend the context length of Llama-3-8B-Instruct from 8K to 80K via QLoRA fine-tuning2 . The entire training cycle is super efficient, which takes 8 hours on one 8xA800 (80G) GPU machine. The resulted model exhibits superior performances across a broad range of evaluation tasks, such as NIHS, topic retrieval, and longcontext language understanding; meanwhile, it also well preserves the original capability over short contexts. The dramatic context extension is mainly attributed to merely 3.5K synthetic training samples generated by GPT-4, which indicates the LLMs’ inherent (yet largely underestimated) potential to extend its original context length. In fact, the context length could be extended far beyond 80K with more computation resources.  | April 30, 2024 | [Paper](https://arxiv.org/abs/2404.19553), [Repo](https://github.com/FlagOpen/FlagEmbedding)|
| (4) **Vibe-Eval: A hard evaluation suite for measuring progress of multimodal language models** - This paper introduces Vibe-Eval: a new open benchmark and framework for evaluating multimodal chat models. Vibe-Eval consists of 269 visual understanding prompts, including 100 of hard difficulty, complete with gold-standard responses authored by experts. Vibe-Eval is open-ended and challenging with dual objectives: (i) vibe checking multimodal chat models for day-to-day tasks and (ii) rigorously testing and probing the capabilities of present frontier models. Notably, the hard set contains > 50% questions that all frontier models answer incorrectly. They explore the nuances of designing, evaluating, and ranking models on ultra challenging prompts. They also discuss trade-offs between human and automatic evaluation, and show that automatic model evaluation using Reka Core roughly correlates to human judgment.  | May 1, 2024 | [Paper](https://publications.reka.ai/reka-vibe-eval.pdf), [Repo](https://github.com/reka-ai/reka-vibe-eval)|
| (5) **PROMETHEUS 2: An Open Source Language Model Specialized in Evaluating Other Language Models** - This paper introduces introduce Prometheus 2, a more powerful evaluator LM than it’s predecessor that closely mirrors human and GPT-4 judgements. The model aim to address the critical shortcomings of proprietary LMs: 1) they issue scores that significantly diverge from those assigned by humans, 2) they lack the flexibility to perform both direct assessment and pairwise ranking, the two most prevalent forms of assessment, and 3) they do not possess the ability to evaluate based on custom evaluation criteria, focusing instead on general attributes like helpfulness and harmlessness. The model is capable of processing both direct assessment and pair-wise ranking formats grouped with a user-defined evaluation criteria. On four direct assessment benchmarks and four pairwise ranking benchmarks, PROMETHEUS 2 scores the highest correlation and agreement with humans and proprietary LM judges among all tested open evaluator LMs.  | May 2, 2024 | [Paper](https://arxiv.org/abs/2405.01535), [Repo](https://github.com/prometheus-eval/prometheus-eval)|
| (6) **FLAME: Factuality-Aware Alignment for Large Language Models** - This paper studies how to make the LLM alignment process more factual, by first identifying factors that lead to hallucination in both alignment steps: supervised fine-tuning (SFT) and reinforcement learning (RL). In particular, they find that training the LLM on new knowledge or unfamiliar texts can encourage hallucination. This makes SFT less factual as it trains on human-labeled data that may be novel to the LLM. Furthermore, reward functions used in standard RL can also encourage hallucination, because it guides the LLM to provide more helpful responses on a diverse set of instructions, often preferring longer and more detailed responses. Based on these observations, the authors propose factuality-aware alignment (FLAME), comprised of factuality-aware SFT and factuality-aware RL through direct preference optimization. Experiments show that the proposed factuality-aware alignment guides LLMs to output more factual responses while maintaining instruction-following capability.  | May 2, 2024 | [Paper](https://arxiv.org/abs/2405.01525)|


## AI Papers of the Week (April 22 - April 28) - 2024
| **Paper**  | **Release Date** | **Links** |
| ------------- | ------------- | ------------- |
| (1) **Many-Shot In-Context Learning** - The paper explores the transition from few-shot to many-shot in-context learning (ICL) for large language models (LLMs), demonstrating substantial performance gains across a range of tasks. It introduces two novel settings: Reinforced ICL, using model-generated rationales instead of human examples, and Unsupervised ICL, which omits rationales and relies solely on domain-specific questions. These methods significantly enhance the model's ability to tackle complex reasoning tasks and overcome pretraining biases, particularly effective in the many-shot regime. The findings also highlight the limitations of next-token prediction loss as an indicator of downstream ICL performance. | April 17, 2024 | [Paper](https://arxiv.org/abs/2404.11018)|
| (2) **Phi-3 Technical Report: A Highly Capable Language Model Locally on Your Phone** - The paper introduces phi-3-mini, a 3.8 billion parameter language model trained on 3.3 trillion tokens, whose overall performance, as measured by both academic benchmarks and internal testing, rivals that of models such as Mixtral 8x7B and GPT-3.5 (e.g., phi-3-mini achieves 69% on MMLU and 8.38 on MT-bench), despite being small enough to be deployed on a phone. The innovation lies entirely in our dataset for training, a scaled-up version of the one used for phi-2, composed of heavily filtered web data and synthetic data. The model is also further aligned for robustness, safety, and chat format. We also provide some initial parameter-scaling results with a 7B and 14B models trained for 4.8T tokens, called phi-3-small and phi-3-medium, both significantly more capable than phi-3-mini (e.g., respectively 75% and 78% on MMLU, and 8.7 and 8.9 on MT-bench). | April 22, 2024 | [Paper](https://arxiv.org/abs/2404.14219)|
| (3) **The Instruction Hierarchy: Training LLMs to Prioritize Privileged Instructions** - The paper argues that one of the primary vulnerabilities underlying these attacks on LLMs is that LLMs often consider system prompts (e.g., text from an application developer) to be the same priority as text from untrusted users and third parties. To address this, they propose an instruction hierarchy that explicitly defines how models should behave when instructions of different priorities conflict. Then proposes an automated data generation method to demonstrate this hierarchical instruction following behavior, which teaches LLMs to selectively ignore lower-privileged instructions. They apply this method to LLMs, showing that it drastically increases robustness—even for attack types not seen during training—while imposing minimal degradations on standard capabilities. | April 19, 2024 | [Paper](https://arxiv.org/abs/2404.13208)|
| (4) **OpenELM: An Efficient Language Model Family with Open-source Training and Inference Framework** - This work releases OpenELM, a decoder-only transformer-based open language model. The OpenELM uses a layer-wise scaling method for efficient parameter allocation within the transformer model, resulting in improved accuracy compared to existing models. Additionally, they have made the entire framework open-source, including training logs, multiple checkpoints, pre-training configurations, and MLX inference code. This extensive release aims to empower and strengthen the open research community, facilitating future research efforts. | April 22, 2024 | [Paper](https://arxiv.org/abs/2404.14619), [Repo](https://github.com/apple/corenet?tab=readme-ov-file)|
| (5) **Multi-Head Mixture-of-Experts** - This work introduces a new architecture enhancing Sparse Mixtures of Experts (SMoE) by integrating a multi-head mechanism. This mechanism divides each token into sub-tokens, which are then processed by a diverse set of experts in parallel. The sub-tokens are subsequently recombined, enriching the model's capacity to process multiple semantic concepts simultaneously. This approach significantly improves expert activation, deepening contextual understanding and reducing overfitting, and is easy to implement alongside other SMoE models. The effectiveness of MH-MoE is demonstrated across various multilingual and multimodal tasks. | April 23, 2024 | [Paper](https://arxiv.org/abs/2404.15045)|
| (6) **Chinchilla Scaling: A replication attempt** - This work examines the computational scaling laws proposed by Hoffmann et al. (2022). They attempt to replicate the third estimation method from Hoffmann's work, which involves fitting a parametric loss function to a reconstruction of data from their plots. The authors find that the reported estimates are inconsistent with Hoffmann's first two estimation methods, fail at fitting the extracted data, and report implausibly narrow confidence intervals—intervals this narrow would require over 600,000 experiments, while Hoffmann's study likely only ran fewer than 500. In contrast, the rederivation of the scaling law using the third approach yields results that are compatible with the findings from the first two estimation procedures described by Hoffmann et al.  | April 15, 2024 | [Paper](https://arxiv.org/abs/2404.10102), [Repo](https://epochai.org/blog/chinchilla-scaling-a-replication-attempt)|
| (7) **How Far Are We to GPT-4V? Closing the Gap to Commercial Multimodal Models with Open-Source Suites** - This work introduces InternVL 1.5, an opensource multimodal large language model (MLLM) to bridge the capability gap between open-source and proprietary commercial models in multimodal understanding. They introduce three simple improvements: (1) Strong Vision Encoder: we explored a continuous learning strategy for the large-scale vision foundation model—InternViT-6B, boosting its visual understanding capabilities, and making it can be transferred and reused in different LLMs. (2) Dynamic High-Resolution: we divide images into tiles ranging from 1 to 40 of 448×448 pixels according to the aspect ratio and resolution of the input images, which supports up to 4K resolution input. (3) High-Quality Bilingual Dataset: we carefully collected a high-quality bilingual dataset that covers common scenes, document images, and annotated them with English and Chinese question-answer pairs, significantly enhancing performance in OCR- and Chineserelated tasks. They evaluate InternVL 1.5 through a series of benchmarks and comparative studies. Compared to both open-source and proprietary models, InternVL 1.5 shows competitive performance, achieving state-of-the-art results in 8 of 18 benchmarks.  | April 25, 2024 | [Paper](https://arxiv.org/abs/2404.16821), [Repo](https://github.com/OpenGVLab/InternVL)|


## AI Papers of the Week (April 15 - April 21) - 2024
| **Paper**  | **Release Date** | **Links** |
| ------------- | ------------- | ------------- |
| (1) **ReFT: Representation Finetuning for Language Models** - The paper introduces Representation Finetuning (ReFT) methods that operate on a frozen base model to learn task-specific interventions on hidden representations. Additionally, it defines a robust instance of the ReFT family, Low-rank Linear Subspace ReFT (LoReFT), which serves as a drop-in replacement for existing Parameter-efficient fine-tuning (PEFT) methods and learns interventions that are 10x-50x more parameter-efficient than prior state-of-the-art PEFTs. It showcases LoReFT across eight commonsense reasoning tasks, four arithmetic reasoning tasks, Alpaca-Eval v1.0, and GLUE. In all these evaluations, LoReFT delivers the best balance of efficiency and performance, and almost always outperforms state-of-the-art PEFTs. | April 4, 2024 | [Paper](https://arxiv.org/abs/2404.03592), [Repo](https://github.com/stanfordnlp/pyreft)|
| (2) **No “Zero-Shot” Without Exponential Data: Pretraining Concept Frequency Determines Multimodal Model Performance** - This work addresses the question: How is the performance of multimodal models on downstream concepts influenced by the frequency of these concepts in their pretraining datasets? The research investigates this across 34 models and five standard pretraining datasets (CC-3M, CC-12M, YFCC-15M, LAION-400M, LAION-Aesthetics), generating over 300GB of data artifacts. It finds that multimodal models require exponentially more data to achieve linear improvements in downstream "zero-shot" performance, following a sample inefficient log-linear scaling trend. Additionally, the study introduces a long-tail test set, the "Let it Wag!" benchmark, to encourage further research. Overall, the findings highlight a substantial need for training data to enhance "zero-shot" generalization capabilities in multimodal models under large-scale training paradigms.  | April 4, 2024 | [Paper](https://arxiv.org/abs/2404.04125), [Repo](https://github.com/bethgelab/frequency_determines_performance)|
| (3) **Leave No Context Behind: Efficient Infinite Context Transformers with Infini-attention** - This work introduces an efficient method to scale Transformer-based Large Language Models (LLMs) to handle infinitely long inputs using bounded memory and computation. The proposed Infini-attention technique enhances the traditional attention mechanism by incorporating compressive memory, masked local attention, and long-term linear attention into a single Transformer block. The effectiveness of this approach is demonstrated through its application in long-context language modeling benchmarks, 1M sequence length passkey context block retrieval, and 500K length book summarization tasks with 1B and 8B LLMs, enabling fast streaming inference with minimal memory overhead.  | April 10, 2024 | [Paper](https://arxiv.org/abs/2404.07143)|
| (4) **Rho-1: Not All Tokens Are What You Need** - This work challenges traditional language model training methods that uniformly apply next-token prediction loss to all tokens. It argues that not all tokens are equally important and introduces a new model, Rho-1, which uses Selective Language Modeling (SLM) to focus on tokens that align better with the desired distribution. Rho-1 scores pretraining tokens using a reference model and trains the language model to focus on tokens with higher excess loss. When continual pretraining on 15B OpenWebMath corpus, Rho-1 yields an absolute improvement in few-shot accuracy of up to 30% in 9 math tasks. After fine-tuning, Rho-1-1B and 7B achieved state-of-the-art results of 40.6% and 51.8% on MATH dataset, respectively - matching DeepSeekMath with only 3% of the pretraining tokens. Furthermore, when pretraining on 80B general tokens, Rho-1 achieves 6.8% average enhancement across 15 diverse tasks, increasing both efficiency and performance of the language model pre-training.  | April 11, 2024 | [Paper](https://arxiv.org/abs/2404.07965#:~:text=Previous%20language%20model%20pre%2Dtraining,important%20for%20language%20model%20training%22), [Repo](https://github.com/microsoft/rho)|
| (5) **CodecLM: Aligning Language Models with Tailored Synthetic Data** - This work presents CodecLM, a framework for adapting large language models (LLMs) to specific task instructions using tailored synthetic data. CodecLM improves instruction-following capabilities in LLMs by selectively generating high-quality data aligned with target instruction distributions. The approach uses an encode-decode mechanism with Self-Rubrics and Contrastive Filtering, achieving superior performance over existing models in multiple instruction-following benchmarks.  | April 8, 2024 | [Paper](https://arxiv.org/abs/2404.05875)|
| (6) **ControlNet++: Improving Conditional Controls with Efficient Consistency Feedback** - The paper presents an advanced approach to enhancing the controllability of text-to-image diffusion models. ControlNet++ improves upon its predecessor by optimizing pixel-level cycle consistency between generated images and input conditions using a novel reward strategy. This efficient method minimizes the memory and time costs associated with traditional image sampling techniques. Extensive experiments show that ControlNet++ significantly improves controllability under various conditional controls. For example, it achieves improvements over ControlNet by 7.9% mIoU, 13.4% SSIM, and 7.6% RMSE, respectively, for segmentation mask, line-art edge, and depth conditions. | April 11, 2024 | [Paper](https://arxiv.org/abs/2404.07987#:~:text=Extensive%20experiments%20show%20that%20ControlNet,art%20edge%2C%20and%20depth%20conditions.), [Repo](https://github.com/liming-ai/ControlNet_Plus_Plus)|
| (7) **VASA-1: Lifelike Audio-Driven Talking Faces Generated in Real Time** - The paper presents VASA-1, a framework for generating realistic talking faces from a single static image and a speech audio clip. VASA-1 produces detailed lip movements and captures a wide range of facial expressions and head motions, enhancing the perception of authenticity and liveliness. It surpasses existing methods in video quality and facial dynamics and supports real-time generation of 512x512 videos at up to 40 FPS with minimal starting latency, marking a significant advancement in real-time interactive systems using lifelike avatars. | April 16, 2024 | [Paper](https://arxiv.org/abs/2404.10667), [Repo](https://www.microsoft.com/en-us/research/project/vasa-1/)|
| (8) **Video2Game: Real-time, Interactive, Realistic and Browser-Compatible Environment from a Single Video** - The paper presents Video2Game, a novel approach that automatically converts videos of real-world scenes into realistic and interactive game environments. At the heart of the system are three core components: (i) a neural radiance fields (NeRF) module that effectively captures the geometry and visual appearance of the scene; (ii) a mesh module that distills knowledge from NeRF for faster rendering; and (iii) a physics module that models the interactions and physical dynamics among objects. The carefully designed pipeline enables the construction of interactable and actionable digital replicas of the real world. The research benchmarks the system on both indoor and large-scale outdoor scenes. They demonstrate that they can produce highly realistic renderings in real-time and build interactive games on top. | April 15, 2024 | [Paper](https://arxiv.org/abs/2404.09833), [Repo](https://github.com/video2game/video2game)|
| (9) **HQ-Edit: A High-Quality Dataset for Instruction-based Image Editing** - The paper introduces HQ-Edit, a dataset designed to enhance image editing models through instruction-based edits. It features around 200,000 edits, created using advanced models like GPT-4V and DALL-E 3. The dataset emphasizes high quality and diversity with detailed text prompts for each image pair, facilitated by a scalable data collection pipeline. In addition, they propose two evaluation metrics, Alignment and Coherence, to quantitatively assess the quality of image edit pairs using GPT-4V. HQ-Edits high-resolution images, rich in detail and accompanied by comprehensive editing prompts, substantially enhance the capabilities of existing image editing models. For example, an HQ-Edit finetuned InstructPix2Pix can attain state-of-the-art image editing performance, even surpassing those models fine-tuned with human-annotated data. | April 15, 2024 | [Paper](https://arxiv.org/abs/2404.09990), [Repo](https://thefllood.github.io/HQEdit_web/)|
