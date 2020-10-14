# IndoNLU 
![Pull Requests Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat) [![GitHub license](https://img.shields.io/badge/license-MIT-blue.svg)](https://github.com/indobenchmark/indonlu/blob/master/LICENSE) [![Contributor Covenant](https://img.shields.io/badge/Contributor%20Covenant-v2.0%20adopted-ff69b4.svg)](code_of_conduct.md)

IndoNLU is a collection of Natural Language Understanding (NLU) resources for Bahasa Indonesia with 12 downstream tasks. We provide the code to reproduce the results and large pre-trained models (IndoBERT and IndoBERT-lite) trained with around 4 billion word corpus (Indo4B), more than 20 GB of text data. This project was initially started by a joint collaboration between universities and industry, such as Institut Teknologi Bandung, Universitas Multimedia Nusantara, The Hong Kong University of Science and Technology, Universitas Indonesia, Gojek, and Prosa.AI.

## Research Paper
IndoNLU has been accepted by AACL-IJCNLP 2020 and you can find the details in our preprint https://arxiv.org/abs/2009.05387.
If you are using any component on IndoNLU including Indo4B, FastText-Indo4B, or IndoBERT in your work, please cite the following paper:
```
@inproceedings{wilie2020indonlu,
  title={IndoNLU: Benchmark and Resources for Evaluating Indonesian Natural Language Understanding},
  author={Bryan Wilie and Karissa Vincentio and Genta Indra Winata and Samuel Cahyawijaya and X. Li and Zhi Yuan Lim and S. Soleman and R. Mahendra and Pascale Fung and Syafri Bahar and A. Purwarianti},
  booktitle={Proceedings of the 1st Conference of the Asia-Pacific Chapter of the Association for Computational Linguistics and the 10th International Joint Conference on Natural Language Processing},
  year={2020}
}
```

## How to contribute to IndoNLU?
Be sure to check the [contributing guidelines](https://github.com/indobenchmark/indonlu/blob/master/CONTRIBUTING.md) and contact the maintainers or open an issue to collect feedbacks before starting your PR.

## 12 Downstream Tasks
- You can check [[Link]](https://github.com/indobenchmark/indonlu/tree/master/dataset)
- We provide train, valid, and test sets. The labels of the test set are masked (no true labels) in order to preserve the integrity of the evaluation. Please submit your predictions to the submission portal at [CodaLab](https://competitions.codalab.org/competitions/26537)

### Examples
- A guide to load IndoBERT model and finetune the model on Sequence Classification and Sequence Tagging task.
- You can check [link](https://github.com/indobenchmark/indonlu/tree/master/examples)

### Submission Format
Please kindly check the [link](https://github.com/indobenchmark/indonlu/tree/master/submission_examples). For each task, there is different format. Every submission file always start with the `index` column (the id of the test sample following the order of the masked test set). 

For the submission, first you need to rename your prediction into `pred.txt`, then zip the file. After that, you need to allow the system to compute the results. You can easily check the progress in your `results` tab.

## Indo4B Dataset
We provide the access to our large pretraining dataset. In this version, we exclude all Twitter tweets due to restrictions of the Twitter Developer Policy and Agreement.
- 23 GB Indo4B Dataset [[Link]](https://storage.googleapis.com/babert-pretraining/IndoNLU_finals/dataset/preprocessed/dataset_wot_uncased_blanklines.tar.xz)

## IndoBERT and IndoBERT-lite Models
- 8 IndoBERT Pretrained Language Model [[Link]](https://huggingface.co/indobenchmark)
  - IndoBERT-base
    - Phase 1  [[Link]](https://huggingface.co/indobenchmark/indobert-base-p1)
    - Phase 2  [[Link]](https://huggingface.co/indobenchmark/indobert-base-p2)
  - IndoBERT-large
    - Phase 1  [[Link]](https://huggingface.co/indobenchmark/indobert-large-p1)
    - Phase 2  [[Link]](https://huggingface.co/indobenchmark/indobert-large-p2)
  - IndoBERT-lite-base
    - Phase 1  [[Link]](https://huggingface.co/indobenchmark/indobert-lite-base-p1)
    - Phase 2  [[Link]](https://huggingface.co/indobenchmark/indobert-lite-base-p2)
  - IndoBERT-lite-large
    - Phase 1  [[Link]](https://huggingface.co/indobenchmark/indobert-lite-large-p1)
    - Phase 2  [[Link]](https://huggingface.co/indobenchmark/indobert-lite-large-p2)

## FastText (Indo4B)
- Will be released soon!

## Leaderboard
- Community Portal and Public Leaderboard [[Link]](https://www.indobenchmark.com/leaderboard.html)
- Submission Portal https://competitions.codalab.org/competitions/26537
