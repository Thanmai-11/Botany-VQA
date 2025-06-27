# Botany-VQA Dataset
[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.15757916.svg)](https://doi.org/10.5281/zenodo.15757916)

[![License: CC BY 4.0](https://img.shields.io/badge/License-CC%20BY%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by/4.0/)

**Botany-VQA** is a Visual Question Answering dataset adapted from the Oxford 102 Flowers dataset. It supports research in domain-specific, low-resource VQA tasks.

##  Files

##  How to Use the Dataset

This repository includes two CSV files containing Visual Question Answering (VQA) data built on top of the **Oxford 102 Flowers** dataset:

| File | Description |
|------|-------------|
| `curated_botany_vqa.csv` | Contains ~12,000 QA pairs generated using structured templates. Focuses on clear, factual questions related to visual and taxonomic features of flowers. |
| `merged_botany_vqa.csv` | Includes ~52,000 QA pairs. Combines the curated QA pairs with more free-form, diverse natural language questions to increase difficulty and realism. |

###  Image Source Requirement

Both CSVs reference image files using the `image_path` column. These filenames correspond to images from the official **Oxford 102 Flowers** dataset.

 To use these QA pairs:
1. Download the original Oxford 102 Flowers dataset from:  
   🔗 https://www.robots.ox.ac.uk/~vgg/data/flowers/102/index.html
2. Make sure the folder structure matches the paths listed in the `image_path` column (e.g., `jpg/image_00001.jpg`)
3. Place the images alongside your CSVs or update the `image_path` accordingly in code

###  CSV Format

Each CSV file includes:
- `image_path`: Relative path to the Oxford 102 Flowers image
- `question`: A natural language VQA question (template or free-form)
- `answer`: The correct answer to the question


- `curated_botany_vqa.csv`: Template-based, factual QA pairs aligned with flower images.
- `merged_botany_vqa.csv`: Extended dataset with diverse, free-form natural language QA pairs.

All QA pairs reference images from the [Oxford 102 Flowers dataset](https://www.robots.ox.ac.uk/~vgg/data/flowers/102/index.html).

##  Statistics

| Dataset      | QA Pairs | Unique Images | Unique Questions | Unique Answers |
|--------------|----------|----------------|------------------|----------------|
| Curated      | 12,000   | 2,000          | 14               | 22             |
| Merged       | 52,000   | 2,000          | 34               | 42             |

## Format

Each row contains:
- `image_path`: Filename of the Oxford Flowers image
- `question`: Natural language question
- `answer`: Ground-truth answer

##  Suggested Use

This dataset can be used to evaluate:
- Transformer-based VQA models
- Cross-domain transfer (e.g., medical → botany)
- Template vs. free-form question understanding
- Multimodal reasoning in low-resource domains

##  License

This dataset is released under the [Creative Commons Attribution 4.0 License (CC BY 4.0)](https://creativecommons.org/licenses/by/4.0/).

##  Citation

If you use this dataset, please cite:

```
Thanmai, “Botany-VQA: Visual Question Answering Dataset for Oxford 102 Flowers,” Zenodo, June 2025. [Online]. Available: https://doi.org/10.5281/zenodo.15757916
```
