# 🏷️ CoNLL-Toolkit

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Python 3.6+](https://img.shields.io/badge/python-3.6+-blue.svg)](https://www.python.org/downloads/)
[![Jupyter Notebook](https://img.shields.io/badge/Jupyter-F37626.svg?&style=flat&logo=Jupyter&logoColor=white)](https://jupyter.org/)

A powerful Jupyter Notebook-based toolkit for effortlessly managing, analyzing, and modifying CoNLL format annotations. Perfect for NLP researchers and practitioners working with named entity recognition (NER) datasets. Please check the CoNLL files in "samples" folder to learn about the compatible formats.

## 📋 Repository Contents
- Jupyter Notebook with CoNLL editing functionality
- Sample CoNLL file (yours.conll)

## ✨ Features

- 📊 **View Annotations**: Instantly visualize all annotations in the CoNLL file along with the total count
- 🏷️ **Label Statistics**: Analyze the distribution of labels in your dataset with detailed counts
- 🔍 **Search Labels**: Find entities with specific labels/tags and track their occurrences
- 🔍 **Search Tokens**: Find entities with specific tokens and track their occurrences
- ✂️ **Remove Labels**: Selectively remove labels from annotations
- 🔄 **Merge Labels**: Combine multiple labels into one
- ✏️ **Rename Labels**: Easily batch rename labels using a dictionary mapping
- ✂️ **Delete Sentences**: Selectively remove sentences containing particular labels
- ✂️ **Delete Useless Sentences**: Remove useless sentences containing no annotations or labels
- ✂️ **Delete Duplicate Sentences**: Remove duplicate sentences

## 🚀 Getting Started

### Prerequisites

- Python 3.6+
- Jupyter Notebook

### Installation

1. Clone the repository:
```bash
git clone https://github.com/SakibAhmedShuva/CoNLL-Toolkit.git
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

# Search Annotations with a specific label
editor.search_by_token("Florida")

# Remove a label
editor.remove_label('O')

# Delete entire sentences containing specific labels
editor.delete_sentences_with_label("B-PER")

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
