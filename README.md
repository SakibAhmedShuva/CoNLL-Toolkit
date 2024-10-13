# 🏷️ CoNLL-Toolkit

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Python 3.6+](https://img.shields.io/badge/python-3.6+-blue.svg)](https://www.python.org/downloads/)
[![Jupyter Notebook](https://img.shields.io/badge/Jupyter-F37626.svg?&style=flat&logo=Jupyter&logoColor=white)](https://jupyter.org/)

A powerful Jupyter Notebook-based toolkit for effortlessly managing, analyzing, and modifying CoNLL format annotations. Perfect for NLP researchers and practitioners working with named entity recognition (NER) datasets.

## 📋 Repository Contents
- Jupyter Notebook with CoNLL editing functionality
- Sample CoNLL file (yours.conll)

## ✨ Features

- 📊 **View Annotations**: Instantly visualize all annotations in the CoNLL file
- 🏷️ **Label Statistics**: Count and analyze the distribution of labels in your dataset
- 🔍 **Smart Search**: Find entities with specific labels
- ✂️ **Remove Labels**: Selectively remove labels from annotations
- 🔄 **Merge Labels**: Combine multiple labels into one
- ✏️ **Rename Labels**: Batch rename labels with a simple dictionary mapping

## 🚀 Getting Started

### Prerequisites

- Python 3.6+
- Jupyter Notebook

### Installation

1. Clone the repository:
```bash
git clone https://github.com/yourusername/CoNLL-Toolkit.git
cd CoNLL-Toolkit
```

2. Install required packages:
```bash
pip install jupyter
```

3. Launch Jupyter Notebook:
```bash
jupyter notebook
```

4. Open the `CoNLL-Toolkit.ipynb` notebook in your browser.

## 💻 Usage

The notebook provides an intuitive interface with the following functionalities:

1. **View Annotations**: Display all annotations in your dataset
2. **Label Statistics**: See a distribution of all labels with their counts
3. **Search Labels**: Find specific labels in your dataset
4. **Remove Labels**: Select and remove unwanted labels
5. **Merge Labels**: Combine multiple labels into one
6. **Rename Labels**: Batch rename labels using a dictionary mapping

### Example Usage

```python
# Initialize the ConllEditor
editor = ConllEditor('yours.conll')

# View annotations
editor.view_annotations()

# Get label statistics
editor.label_stats()

# Search for a specific label
editor.search_by_label('B-PER')

# Remove a label
editor.remove_label('O')

# Merge labels
editor.merge_labels(['B-PER', 'I-PER'], 'PER')

# Rename labels
editor.rename_labels({'B-ORG': 'B-COMPANY', 'I-ORG': 'I-COMPANY'})

# Save the modified file
editor.save('modified_yours.conll')
```

## 🤝 Contributing

Contributions to this project are welcome. Please feel free to submit a Pull Request.

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- Inspired by the needs of the NLP community
- Built with Python and Jupyter Notebook


## 🌐 Connect with Me

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://linkedin.com/in/sakibahmedai)
[![Kaggle](https://img.shields.io/badge/Kaggle-20BEFF?style=for-the-badge&logo=kaggle&logoColor=white)](https://kaggle.com/skbahmed)
[![LeetCode](https://img.shields.io/badge/LeetCode-FFA116?style=for-the-badge&logo=leetcode&logoColor=black)](https://leetcode.com/SakibAhmedShuva)
[![Email](https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:sakibahmedbup@gmail.com)
