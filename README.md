# 🏦 Banking77 Intent Classification with DistilBERT

A fine-tuned **DistilBERT** model for classifying banking customer support queries into **77 intent categories** using the [Banking77](https://huggingface.co/datasets/banking77) dataset.

---

## 📊 Results

| Metric | Score |
|---|---|
| **Accuracy** | 86.92% |
| **F1 Score (weighted)** | 86.36% |
| Training Epochs | 5 |
| Dataset Size | 13,083 samples |
| Number of Classes | 77 |

---

##  Model

| Property | Value |
|---|---|
| Base Model | `distilbert-base-uncased` |
| Task | Multi-class Text Classification |
| Framework | HuggingFace Transformers + PyTorch |
| Training Hardware | NVIDIA GeForce RTX 5060 (8GB) |

---

##  Project Structure

```
banking77-classifier/
├── README.md
├── train.py                  # Training script
├── predict.py                # Inference script
├── model/                    # Saved model files
│   ├── config.json
│   ├── model.safetensors
│   ├── tokenizer_config.json
│   ├── tokenizer.json
│   └── vocab.txt
└── requirements.txt
```

---

##  Dataset

The [Banking77](https://huggingface.co/datasets/banking77) dataset contains 13,083 customer service queries from the banking domain, labeled across 77 fine-grained intent classes.

**Sample classes:**
- `activate_my_card`
- `card_arrival`
- `transaction_charged_twice`
- `declined_cash_withdrawal`
- `transfer_fee_charged`
- `edit_personal_details`
- ... and 71 more
