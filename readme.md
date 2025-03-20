## (ICASSP Oral 2025) NECHO v2: Overcoming Uncertain Incompleteness for Robust Multimodal Sequential Diagnosis Prediction via Curriculum Data Erasing Guided Knowledge Distillation

**[Heejoon Koo<sup>1</sup>](https://scholar.google.co.kr/citations?user=93HqsvAAAAAJ&hl=ko)**
<br>
<sup>1</sup>University College London
<br>

This paper has been designated as a **Lecture (Oral) Presentation** in the **Bioinformatics and Neural Signals** track, and we sincerely appreciate.


<a href='https://ieeexplore.ieee.org/abstract/document/10890473'><img src='https://a11ybadges.com/badge?logo=ieee'></a>
<a href='https://arxiv.org/abs/2407.19540'><img src='https://a11ybadges.com/badge?logo=arxiv'></a> 




## 📋 Announcements
- [2025.03.20] The remaining code and checkpoint files will be updated soon. We appreciate your understanding and patience in the meantime!



## 1. Install Packages

All experiments in this paper were conducted using CUDA 11 on a single NVIDIA A6000 GPU, which necessitates at least 48GB of video memory to run successfully.

```
pip install torch==1.12.1+cu113 torchvision==0.13.1+cu113 torchaudio==0.12.1 --extra-index-url https://download.pytorch.org/whl/cu113
pip install transformers==4.31.0
pip install numpy==1.23.2
pip install pandas==1.5.3
pip install -U scikit-learn
pip install scikit-multilearn==0.2.0
pip install scipy==1.12
pip install gensim
```


## 2. Download Dataset

Please download MIMIC-III dataset from [official PhysioNet link](https://physionet.org/content/mimiciii/1.4/), unzip it, and place the required files as indicated.

This repository includes both the ```ccs_multi_dx_tool_2015.csv``` and ```ccs_single_dx_tool_2015.csv``` files. Detailed information regarding these files is available in the CCS Users Guide, which can be accessed [here](https://hcup-us.ahrq.gov/toolssoftware/ccs/CCSUsersGuide.pdf).

```
NECHOv2/
├── data
│   └── mimic-iii
│       │   ccs_multi_dx_tool_2015.csv
│       │   ccs_single_dx_tool_2015.csv
│       │   ADMISSIONS.csv
│       │   DIAGNOSES_ICD.csv
│       │   NOTEEVENTS.csv
│       └── PATIENTS.csv
└── MIMIC-III Data Preprocessing for Next Visit Diagnosis Prediction.ipynb

```

## 3. Preprocess Dataset

Execute the ```MIMIC-III Data Preprocessing for Next Visit Diagnosis Prediction.ipynb``` notebook to generate all necessary files in the required directory.


<br>

## 😉 Citation
If you find our work helpful, please leave us a star and cite our paper(s).

```
@inproceedings{koo2024next,
  title={Next Visit Diagnosis Prediction via Medical Code-Centric Multimodal Contrastive EHR Modelling with Hierarchical Regularisation},
  author={Koo, Heejoon},
  booktitle={Findings of the Association for Computational Linguistics: EACL 2024},
  pages={41--55},
  year={2024}
}

```

```
@inproceedings{koo2025overcoming,
  title={Overcoming Uncertain Incompleteness for Robust Multimodal Sequential Diagnosis Prediction via Curriculum Data Erasing Guided Knowledge Distillation},
  author={Koo, Heejoon},
  booktitle={ICASSP 2025-2025 IEEE International Conference on Acoustics, Speech and Signal Processing (ICASSP)},
  pages={1--5},
  year={2025},
  organization={IEEE}
}
```