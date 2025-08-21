# Data-Driven Approaches for Identifying Depression Severity in Social Media Posts

This repository contains LaTeX source files and compiled PDF, as well as Python experiment notebooks and the datasets used for the paper, prepared as the final project for my *Natural Language Processing* class.

The topic of this paper is associated with the [**RANLP 2025 shared task: Identification of the Severity of Depression in Forum Posts**](https://ranlp.org/ranlp2025/index.php/shared-task/).

You can read the full paper [here](docs/paper.pdf).

## Abstract
In this study, I explored different approaches to classify depression severity from social media text. I combined multiple publicly available datasets to build a unique dataset labeled with three severity levels: not depression, moderate, and severe.
I evaluated traditional machine learning models using ***TF-IDF*** and ***sentence embeddings***, deep learning models based on ***BiLSTM*** with pre-trained ***GloVe*** embeddings, and a fine-tuned ***DistilBERT*** transformer model, pre-trained with ***masked language modeling***.

My results show that simple traditional models with strong features perform best, while deep learning models faced challenges likely due to limited and imbalanced data.
The ***DistilBERT*** model performed competitively but requires more fine-tuning and data augmentation to reach its full potential.
I conclude that, given current data constraints, simpler models remain strong baselines, and future work should focus on collecting richer data and improving augmentation and fine-tuning methods for advanced models.

## Datasets
The repository includes a custom dataset I created by cleaning and merging multiple publicly available datasets on depression detection from social media.

All original datasets remain the property of their respective authors. Please refer to their licenses and publications for proper citation:
- [DEPSEV](https://github.com/usmaann/Depression_Severity_Dataset)
- [DEPSIGN](https://github.com/rafalposwiata/depression-detection-lt-edi-2022/tree/main/data/original_dataset)
- [Reddit Depression Corpora](https://github.com/rafalposwiata/depression-detection-lt-edi-2022/tree/main/data/reddit_depression_corpora)

The [merged dataset](data/depset.csv) is provided for **research and educational purposes only**. If you use it, please cite the original datasets in addition to this work.

## Citation
If you want to cite this paper in your work, please use the following:
```bibtex
@misc{Uifalean2025DepSeverity,
  title       = {Data-Driven Approaches for Identifying Depression Severity in Social Media Posts},
  author      = {Paul-Adrian Uifalean},
  year        = {2025},
  institution = {Babes-Bolyai University},
  note        = {NLP course project},
  url         = {https://github.com/paulicuu/depsev-analysis}
}
```

## License
The paper is licensed under the [Creative Commons Attribution 4.0 International License (CC BY 4.0)](https://creativecommons.org/licenses/by/4.0/).

The source code and notebooks are licensed under the [MIT License](https://opensource.org/license/MIT).
