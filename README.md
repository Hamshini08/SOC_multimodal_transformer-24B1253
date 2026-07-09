# Vision Language Model from Scratch

A complete PyTorch implementation of a Vision Language Model (VLM) developed as part of the **Seasons of Code 2026** program. The project builds modern vision-language systems from first principles, starting with a simple language model and progressively implementing transformers, Vision Transformers, multimodal contrastive learning, retrieval, and downstream applications.

---

## Project Roadmap

### Task 0 — PyTorch Fundamentals
- Tensor operations and automatic differentiation
- Building simple neural networks
- Training and optimization pipeline

### Task 1 — Transformer from Scratch
- Multi-head self-attention
- Positional embeddings
- Residual connections
- Layer Normalization
- Feed-forward networks
- Autoregressive text generation

### Task 2 — Understanding Attention
- Self-attention implementation
- Attention visualization
- Residual and LayerNorm ablations

### Task 3 — Vision Transformer (ViT)
- Image patch embedding
- CLS token
- Positional embeddings
- Transformer encoder
- CIFAR-10 image classification

### Task 4 — Cross Attention
- Cross-attention module
- Vision-language fusion
- Attention map visualization

### Task 5 — Contrastive Learning (CLIP)
- Dual encoder architecture
- Image encoder (ViT)
- Text encoder (Transformer)
- InfoNCE loss
- Image-text alignment

### Task 6 — Vision Language Model
- Flickr8k training
- Retrieval evaluation
- Similarity map visualization
- Zero-shot classification
- Text-to-image search engine

---

## Repository Structure

```text
.
├── task0/
├── task1/
├── task2/
├── task3/
├── task4/
├── task5/
├── task6/
│
│
├── requirements.txt
└── README.md
```

---

## Final Results

### CLIP Training

| Metric | Value |
|--------|------:|
| Final Train Loss | **0.1953** |
| Final Validation Loss | **1.8113** |
| Convergence | **~8000 steps** |

### Retrieval Performance

| Task | Recall@1 | Recall@5 | Recall@10 |
|------|---------:|---------:|----------:|
| Image → Text | **20.68%** | **45.25%** | **56.75%** |
| Text → Image | **19.31%** | **42.47%** | **54.49%** |

---

## Applications

- Image ↔ Text Retrieval
- Similarity Map Visualization
- Zero-Shot Image Classification
- Text-to-Image Semantic Search

---

## Installation

```bash
git clone <[repository-url](https://github.com/Hamshini08/SOC_multimodal_transformer-24B1253)>

cd Vision-Language-Model
```

```bash
pip install -r requirements.txt
```

---

## Running the Project

### Transformer

```bash
python task1/train.py
```

### Vision Transformer

```bash
python task3/train.py
```

### CLIP Training

```bash
python task6/train.py
```

### Retrieval Evaluation

```bash
python task6/eval.py
```

### Similarity Maps

```bash
python task6/qualitative.py
```

### Zero-Shot Classification

```bash
python task6/zero_shot.py
```

### Text-to-Image Search

```bash
python task6/text_to_image_search.py
```

---

## Dependencies

See `requirements.txt`.

---
## Checkpoint

The trained CLIP-style model checkpoint (`best_model.pt`) is included in the repository. If GitHub's file size limit is exceeded, it can alternatively be hosted on Google Drive with a download link.

---

## Technologies Used

- Python
- PyTorch
- torchvision
- NumPy
- Matplotlib
- Pillow
- tqdm
- ipywidgets

---

## Acknowledgements

This project was completed as part of the **Seasons of Code 2026** program organised by Web and Coding Club (WnCC), IIT Bombay.

## Author

**Hamshini Kanuri**

Undergraduate

Department of Electrical Engineering  

Indian Institute of Technology Bombay

Seasons of Code 2026
