# SemiHVision: Enhancing Medical Multimodal Models with a Semi-Human Annotated Dataset and Fine-Tuned Instruction Generation

Multimodal large language models (MLLMs) have made significant strides, yet they face challenges in the medical domain due to limited specialized knowledge. While recent medical MLLMs demonstrate strong performance in lab settings, they often struggle in real-world applications, highlighting a substantial gap between research and practice. In this paper, we seek to address this gap at various stages of the end-to-end learning pipeline, including data collection, model fine-tuning, and evaluation. At the data collection stage, we introduce SemiHVision, a dataset that combines human annotations with automated augmentation techniques to improve both medical knowledge representation and diagnostic reasoning. For model fine-tuning, we trained PMC-Cambrian-8B-AN over 2400 H100 GPU hours, resulting in performance that surpasses public medical models like HuatuoGPT-Vision-34B (79.0% vs. 66.7%) and private general models like Claude3-Opus (55.7%) on traditional benchmarks such as SLAKE and VQA-RAD. In the evaluation phase, we observed that traditional benchmarks cannot accurately reflect realistic clinical task capabilities. To overcome this limitation and provide more targeted guidance for model evaluation, we introduce the JAMA Clinical Challenge, a novel benchmark specifically designed to evaluate diagnostic reasoning. On this benchmark, PMC-Cambrian-AN achieves state-of-the-art performance with a GPT-4 score of 1.29, significantly outperforming HuatuoGPT-Vision-34B (1.13) and Claude3-Opus (1.17), demonstrating its superior diagnostic reasoning abilities.


# Distribution

![Image text](https://github.com/believewhat/SemiHVision/blob/main/distribution.png)

# Datsets Links
[Dataset Link](https://huggingface.co/datasets/akemiH/Med-Instruction)

# Data Resource

| Dataset               | Caption Available | Link  | License                                             |
|-----------------------|-----------|-------|-----------------------------------------------------|
| Deeplesion                   | Yes       | [Link](https://huggingface.co/datasets/farrell236/DeepLesion) | -                                                   |
| PadChest        | Yes       | [Link](https://bimcv.cipf.es/bimcv-projects/padchest/) | PADCHEST Dataset Research Use Agreement                                           |
| Eurorad  | Yes       | [Link](https://www.eurorad.org/) | Creative Commons Attribution 4.0 International License                                   |
| MIMIC-CXR-JPG          | No       | [Link](https://physionet.org/content/mimic-cxr-jpg/2.1.0/) | PhysioNet Credentialed Health Data License 1.5.0                                           |
| LLD              | Yes        | [Link](https://github.com/LMMMEng/LLD-MMRI-Dataset?tab=readme-ov-file) | LLD-MMRI Agreement  |
| MAMA-MIA                  | Yes       | [Link](https://www.synapse.org/Synapse:syn60868042/wiki/628716) | CC BY-NC-SA 4.0                                     |
| PMC-VQA                   | Yes       | [Link](https://huggingface.co/datasets/xmcmic/PMC-VQA) | CC BY-SA                                           |
| PMC-Instruct            | Yes       | - | OpenRAIL                                           |
| Quilt               | Yes       | [Link](https://zenodo.org/records/8239942) | -                                     |
| Radiopaedia                | No       | [Link](https://radiopaedia.org/?lang=us) | Radiopaedia Agreement                                             |
| JAMA Clinical Challenge                | No        | [Link](https://jamanetwork.com/collections/44038/clinical-challenge) | JAMA's Angreement                                     |
| LLaVA-Med             | Yes       | [Link](https://github.com/LMMMEng/LLD-MMRI-Dataset) | CC BY NC 4.0                                        |


## Disclaimer

The dataset provided (referred to as "This Dataset") is constructed using multiple publicly available datasets and is intended solely for academic and technical research by researchers and developers. Any individual or organization (hereinafter referred to as "User") accessing or using this dataset must comply with the following disclaimer:

### Dataset Source:
This Dataset is built from several publicly available datasets. The sources and licenses of these datasets are clearly stated in the accompanying documentation. Users are required to adhere to the relevant licenses, terms of use, and restrictions specified by the original dataset providers. For cases published on the EuroRad website prior to July 6, 2015, these do not fall under the Creative Commons Attribution 4.0 International License. Therefore, Users must obtain direct permission from the author who submitted the case for any use. To avoid complications, we recommend not using cases published before this date, unless you can secure explicit permission from each case submitter for every intended use.


### Data Accuracy:
Reasonable efforts have been made to ensure the accuracy, integrity, and completeness of This Dataset. However, the User assumes all risks associated with using the dataset. The providers of This Dataset accept no responsibility for any errors, inaccuracies, or omissions that may arise.

### Limitation of Liability:
Under no circumstances shall the providers or contributors of This Dataset be liable for any damages or consequences arising from the use or misuse of This Dataset by the User.

### Usage Restrictions:
Users of This Dataset must comply with all applicable laws, regulations, and ethical standards. The dataset must not be used for illegal purposes, privacy violations, defamation, discrimination, or other unethical activities.

### Intellectual Property:
The intellectual property rights of the original image data in This Dataset belong to the respective rights holders of the source datasets. Users must not engage in activities that violate these intellectual property rights.

### Ethical Use:
As a non-profit organization, we promote a collaborative and ethical open-source environment. Should any content within This Dataset infringe upon legitimate rights, please contact us, and we will make every effort to resolve the issue.

By downloading, accessing, or using This Dataset, the User acknowledges that they have read, understood, and agreed to comply with this disclaimer. If the User does not accept any part of this disclaimer, they should refrain from using This Dataset.



```
@article{wang2024semihvision,
  title={SemiHVision: Enhancing Medical Multimodal Models with a Semi-Human Annotated Dataset and Fine-Tuned Instruction Generation},
  author={Wang, Junda and Ting, Yujan and Chen, Eric Z and Tran, Hieu and Yu, Hong and Huang, Weijing and Chen, Terrence},
  journal={arXiv preprint arXiv:2410.14948},
  year={2024}
}
```
