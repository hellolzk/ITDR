## ITDR: An Instruction Tuning Dataset for Enhancing Large Language Models in Recommendations

 [*Paper*](https://arxiv.org/abs/2508.05667)

## Model

The modles are available at [*ModelScope*](https://www.modelscope.cn/profile/lzkhhh). 

## Introduction

Large language models (LLMs) have demonstrated outstanding performance in natural language processing tasks. However, in the field of recommendation systems, due to the structural differences between user behavior data and natural language, LLMs struggle to effectively model the associations between user preferences and items. Although prompt-based methods can generate recommendation results, their inadequate     understanding of recommendation tasks leads to constrained performance. To address this gap, in this work, we construct a sufficient instruction tuning dataset, ITDR, which encompasses 7 subtasks across two core root tasks—useritem interaction and user-item understanding. The dataset integrates data from 13 public recommendation datasets and is built using manually crafted standardized templates, comprising approximately 200,000 instances. Experimental results demonstrate that ITDR significantly enhances the performance of mainstream open-source LLMs such as GLM-4, Qwen2.5, Qwen2.5-Instruct and LLaMA-3.2 on recommendation tasks. Furthermore, we analyze the correlations between tasks and explore the impact of task descriptions and data scale on instruction tuning effectiveness. Finally, we perform comparative experiments against closed-source LLMs with substantial parameters.

## Architecture of ITDR

<img width="2196" height="1556" alt="academic_sankey" src="https://github.com/user-attachments/assets/15f7c9a8-0c65-407d-ace8-bbe0a4451a08" />

## Perfomance

<img width="4770" height="1999" alt="Comparison_before_and_after_fine-tuning" src="https://github.com/user-attachments/assets/6eb238a1-43bc-4f2a-93be-10c152c945ed" />

## All Source Data We Used In The Paper

| Dataset Name | Link |
|--------------|------|
| Anime Dataset 2023     | [https://www.kaggle.com/datasets/dbdmobile/myanimelist-dataset](https://www.kaggle.com/datasets/dbdmobile/myanimelist-dataset) |
| MovieLens 1M/32M     | [https://grouplens.org/datasets/movielens/](https://grouplens.org/datasets/movielens/) |
| Amazon Reviews 2023     | [https://huggingface.co/datasets/McAuley-Lab/Amazon-Reviews-2023/tree/main](https://huggingface.co/datasets/McAuley-Lab/Amazon-Reviews-2023/tree/main) |
| MicroLens     | [https://github.com/westlake-repl/MicroLens](https://github.com/westlake-repl/MicroLens) |
| PixelRec     | [https://github.com/westlake-repl/PixelRec](https://github.com/westlake-repl/PixelRec) |
| BookCrossing     | [https://www.kaggle.com/datasets/ruchi798/bookcrossing-dataset](https://www.kaggle.com/datasets/ruchi798/bookcrossing-dataset) |
| Amazon Books Reviews     | [https://www.kaggle.com/datasets/mohamedbakhet/amazon-books-reviews?select=books_data.csv](https://www.kaggle.com/datasets/mohamedbakhet/amazon-books-reviews?select=books_data.csv) |
| MIND     | [https://msnews.github.io/](https://msnews.github.io/) |
| Steam     | [https://github.com/kang205/SASRec?tab=readme-ov-file](https://github.com/kang205/SASRec?tab=readme-ov-file) |
| Yelp     | [https://www.kaggle.com/datasets/yelp-dataset/yelp-dataset](https://www.kaggle.com/datasets/yelp-dataset/yelp-dataset) |
| Last.FM 360K     | [http://ocelma.net/MusicRecommendationDataset/lastfm-360K.html](http://ocelma.net/MusicRecommendationDataset/lastfm-360K.html) |
| Last.FM 1K   | [https://yann.lecun.com/exdb/mnist/](http://ocelma.net/MusicRecommendationDataset/lastfm-1K.html)|
