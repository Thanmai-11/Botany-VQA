# Botany-VQA Dataset

[![License: CC BY 4.0](https://img.shields.io/badge/License-CC%20BY%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by/4.0/)

**Botany-VQA** is a Visual Question Answering dataset adapted from the Oxford 102 Flowers dataset. It supports research in domain-specific, low-resource VQA tasks.

##  Files

- `curated_botany_vqa.csv`: Template-based, factual QA pairs aligned with flower images.
- `merged_botany_vqa.csv`: Extended dataset with diverse, free-form natural language QA pairs.

All QA pairs reference images from the [Oxford 102 Flowers dataset](https://www.robots.ox.ac.uk/~vgg/data/flowers/102/index.html).

##  Statistics

| Dataset      | QA Pairs | Unique Images | Unique Questions | Unique Answers |
|--------------|----------|----------------|------------------|----------------|
| Curated      | 12,000   | 2,000          | 14               | 22             |
| Merged       | 52,000   | 2,000          | 34               | 42             |

##  Format

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
Thanmai, “Botany-VQA: Visual Question Answering Dataset for Oxford 102 Flowers,” Zenodo, 2024. [Online]. Available: https://doi.org/xxxxx
```
