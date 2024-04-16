# AI Papers of The Week

As a researcher, I frequently read AI papers and am trying to create this repository to record some highlighted AI papers that I read each week.

Here is the weekly series:

## 2024

- [AI Papers of the Week (April 15 - April 21)](./#ai-papers-of-the-week-april-15---april-21---2024)

## AI Papers of the Week (April 15 - April 21) - 2024
| **Paper**  | **Links** |
| ------------- | ------------- |
| (1) **ReFT: Representation Finetuning for Language Models** - The paper introduces Representation Finetuning (ReFT) methods that operate on a frozen base model to learn task-specific interventions on hidden representations. Additionally, it defines a robust instance of the ReFT family, Low-rank Linear Subspace ReFT (LoReFT), which serves as a drop-in replacement for existing Parameter-efficient fine-tuning (PEFT) methods and learns interventions that are 10x-50x more parameter-efficient than prior state-of-the-art PEFTs. It showcases LoReFT across eight commonsense reasoning tasks, four arithmetic reasoning tasks, Alpaca-Eval v1.0, and GLUE. In all these evaluations, LoReFT delivers the best balance of efficiency and performance, and almost always outperforms state-of-the-art PEFTs.  | [Paper](https://arxiv.org/abs/2404.03592), [Repo](https://github.com/stanfordnlp/pyreft)|
| (2) **No “Zero-Shot” Without Exponential Data: Pretraining Concept Frequency Determines Multimodal Model Performance** - This work addresses the question: How is the performance of multimodal models on downstream concepts influenced by the frequency of these concepts in their pretraining datasets? The research investigates this across 34 models and five standard pretraining datasets (CC-3M, CC-12M, YFCC-15M, LAION-400M, LAION-Aesthetics), generating over 300GB of data artifacts. It finds that multimodal models require exponentially more data to achieve linear improvements in downstream "zero-shot" performance, following a sample inefficient log-linear scaling trend. Additionally, the study introduces a long-tail test set, the "Let it Wag!" benchmark, to encourage further research. Overall, the findings highlight a substantial need for training data to enhance "zero-shot" generalization capabilities in multimodal models under large-scale training paradigms.  | [Paper]([https://arxiv.org/abs/2404.03592](https://arxiv.org/abs/2404.04125)), [Repo](https://github.com/bethgelab/frequency_determines_performance)|
