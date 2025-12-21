# Stack Overflow Question Popularity Classifier

[![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)](https://www.python.org/downloads/)
[![PyTorch](https://img.shields.io/badge/PyTorch-2.0+-red.svg)](https://pytorch.org/)
[![License](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)

> Predicting the popularity of Stack Overflow questions using fine-tuned MiniLM model

---

### Abstract

Stack Overflow is designed as a knowledge base rather than a support forum; therefore, the community prioritizes concise, technical accuracy over friendly social interaction. Many users stumble at the first hurdle-namely, providing enough context as they fail to include a minimal reproducible example, leaving others to guess while trying to debug the code. Or just as bad, they describe the issue from their own perspective only, expecting the community to magically find the answer. Aimed at improving platform efficiency, this project classifies Stack Overflow questions into four popularity tiers using a fine-tuned MiniLM. The methodology specifically tackles severe class imbalance through weighted loss functions, resulting in a macro F1-score of 0.40. This 'automated critic' allows users to gauge their question's potential and make necessary adjustments before hitting 'Post', ensuring better engagement.

**Key Features:**
- BERT-based text classification (MiniLM)
- Handles 27:1 class imbalance ratio
- Transfer learning from pretrained models
- Comprehensive evaluation metrics

### Future Work

- [ ] Implement Focal Loss for better minority class performance
- [ ] Add temporal features (post date, trending topics)
- [ ] Use CodeBERT for better code understanding
- [ ] Ensemble multiple models
- [ ] Deploy as web API

### Citation

If you use this code in your research, please cite:
```bibtex
@misc{stackoverflow-popularity-2025,
  author = {Your Name},
  title = {Stack Overflow Question Popularity Classification Using Fine-Tuned MiniLM},
  year = {2025},
  publisher = {GitHub},
  url = {https://github.com/yourusername/stackoverflow-popularity-classifier}
}
```

### Acknowledgments

- Dataset: [Stack Overflow Questions Dataset](https://huggingface.co/datasets/pacovaldez/stackoverflow-questions)
- Pretrained Model: [MiniLM](https://huggingface.co/microsoft/MiniLM-L12-H384-uncased)
- Inspired by research in imbalanced text classification

---
> **Note:** While this project's code is MIT licensed, the dataset and model may have their own specific usage terms.
