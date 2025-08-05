## ITDR: An Instruction Tuning Dataset for Enhancing Large Language Models in Recommendations

## Introduction

Large language models (LLMs) have demonstrated outstanding performance in natural language processing tasks. However, in the field of recommendation systems, due to the structural differences between user behavior data and natural language, LLMs struggle to effectively model the associations between user preferences and items. Although prompt-based methods can generate recommendation results, their inadequate     understanding of recommendation tasks leads to constrained performance. To address this gap, in this work, we construct a sufficient instruction tuning dataset, ITDR, which encompasses 7 subtasks across two core root tasks—useritem interaction and user-item understanding. The dataset integrates data from 13 public recommendation datasets and is built using manually crafted standardized templates, comprising approximately 200,000 instances. Experimental results demonstrate that ITDR significantly enhances the performance of mainstream open-source LLMs such as GLM-4, Qwen2.5, Qwen2.5-Instruct and LLaMA-3.2 on recommendation tasks. Furthermore, we analyze the correlations between tasks and explore the impact of task descriptions and data scale on instruction tuning effectiveness. Finally, we perform comparative experiments against closed-source LLMs with substantial parameters.

## Architecture of ITDR

![img](file:///F:/研究生/AAAI/绘图/数据规模桑吉_旭日图/academic_sankey.png)

## Perfomance

![Comparison_before_and_after_fine-tuning](F:\研究生\AAAI\绘图\微调前后指标对比\Comparison_before_and_after_fine-tuning.png)

## Model

The modles are available at [*ModelScope*](https://www.modelscope.cn/profile/lzkhhh). 
