## ITDR: An Instruction Tuning Dataset for Enhancing Large Language Models in Recommendations

 [*Paper*](https://arxiv.org/abs/2508.05667)

## 🤖Model

The modles are available at [*ModelScope*](https://www.modelscope.cn/profile/lzkhhh). 
All fine-tuned LoRA adapters are available via [*Google Drive*](https://drive.google.com/drive/folders/1sCCUo1d3bEIVIoRyxN2DnAP0PlkwfTfj?usp=sharing). 
## 🔥News
* **[Nov. 2025]**: **ITDR** has been accepted to **KDD2026**!

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

## The statistics of ITDR
<img width="1098" height="1553" alt="statistics_of_datasets" src="https://github.com/user-attachments/assets/f9f5f1cc-5f98-4dee-9e8f-bbc0545b532d" />

## Details of the main experimental results 
<img width="1152" height="1152" alt="Performance on the user-item interaction tasks" src="https://github.com/user-attachments/assets/6ed84f4f-201b-48e9-86b8-68e23d2157a7" />
<img width="1128" height="912" alt="Performance on the user-item understanding tasks1" src="https://github.com/user-attachments/assets/b8706275-6043-4d9e-b2d4-255e8d4c0046" />
<img width="1143" height="1458" alt="Performance on the user-item understanding tasks2" src="https://github.com/user-attachments/assets/79c1a184-3a9f-45de-83dd-7a03c60f7f04" />

## Details of the root tasks ablation experiment results
<img width="1131" height="1149" alt="remove different root tasks_uii" src="https://github.com/user-attachments/assets/5e3859c1-b0f9-45a8-a2fd-39baaa078cda" />
<img width="1119" height="987" alt="remove different root tasks_uiu1" src="https://github.com/user-attachments/assets/2ea2a2e7-43c3-4dad-b7f6-bae5f0bc47f5" />
<img width="1035" height="1458" alt="remove different root tasks_uiu2" src="https://github.com/user-attachments/assets/d5ad6ac8-51c5-4848-b37e-ad2b6ba95dd8" />

## Details of the subtasks ablation experiment results
<img width="1125" height="1149" alt="subtasks_ablation_uii" src="https://github.com/user-attachments/assets/c3e8f308-e159-4928-8590-da4ab7ce95b9" />
<img width="1131" height="990" alt="subtasks_ablation_uiu1" src="https://github.com/user-attachments/assets/c886d490-1ba8-4e93-b1dd-2019e978520c" />
<img width="1134" height="1416" alt="subtasks_ablation_uiu2" src="https://github.com/user-attachments/assets/57e9904a-fcee-49b0-8f15-bb34144a8a23" />

## Details of experimental results for closed source LLMs
<img width="711" height="1089" alt="closed_source LLMs_uii" src="https://github.com/user-attachments/assets/3a43469d-4f8c-4dd0-bfec-890646b06822" />
<img width="798" height="927" alt="closed_source LLMs_uiu1" src="https://github.com/user-attachments/assets/d71571bf-0673-4d27-8b91-8ee9c470fd40" />
<img width="705" height="1425" alt="closed_source LLMs_uiu2" src="https://github.com/user-attachments/assets/82e03def-6f2e-4765-9b87-c6180f101fe8" />

## Data examples
<img width="1245" height="357" alt="RT" src="https://github.com/user-attachments/assets/7517f273-5fe0-4260-ac70-97bfa80206d0" />
<img width="1242" height="924" alt="TKR" src="https://github.com/user-attachments/assets/38bddc8a-4de6-4e2c-b37b-ccbdae830d58" />
<img width="1242" height="1248" alt="CDR" src="https://github.com/user-attachments/assets/acfbd994-5fe0-4238-9648-901f3661a826" />
<img width="1239" height="375" alt="NIR" src="https://github.com/user-attachments/assets/918d8e63-3a3e-492f-877d-406a6739d3e2" />
<img width="1239" height="453" alt="UAP" src="https://github.com/user-attachments/assets/8db04bce-0541-4054-84a0-102e3b01da4a" />
<img width="1236" height="749" alt="IR" src="https://github.com/user-attachments/assets/fc6e62b2-1a2e-435f-8e3c-c8534da8d559" />
<img width="1233" height="675" alt="TUI" src="https://github.com/user-attachments/assets/f3494a1d-286a-4ae2-a0e5-e11e147fb65e" />

