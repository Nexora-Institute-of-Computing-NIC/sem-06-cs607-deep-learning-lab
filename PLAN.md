# CS607 — Deep Learning Lab — PLAN

**Semester:** 6 · **Credits:** 2 · **Level:** Advanced
**Theory:** 0 hrs · **Lab:** 45 hrs · **Tools:** Python, PyTorch, torchvision, Hugging Face, Weights & Biases (free tier), Jupyter

## Course Format
Pure hands-on. Every lab trains a real model, logs metrics, and writes a short report. Parallel companion to CS601.

## Lab Modules

### Module 1 — Neural Network Foundations (3 labs)
1. Backpropagation from scratch in NumPy on a two-layer network
2. Same network in PyTorch — compare code and results
3. Activations, initialisation, and optimisers — ablation study

### Module 2 — Computer Vision (4 labs)
4. Train a CNN on MNIST — baseline and improvements
5. Train a CNN on CIFAR-10 — augmentation, batch norm, dropout
6. Transfer learning — fine-tune ResNet on a custom 5-class dataset
7. Data augmentation as an ablation — measure accuracy gain

### Module 3 — Sequence Models (3 labs)
8. Train an RNN and LSTM language model on a small corpus
9. Implement attention from scratch
10. Fine-tune a small transformer (BERT or DistilBERT) for classification

### Module 4 — Generative Models (2 labs)
11. Train a VAE on MNIST — sample and interpolate
12. Train a small GAN on MNIST — sample gallery

### Module 5 — Deployment and Analysis (3 labs)
13. Quantise a trained model and measure speed/accuracy
14. Deploy a trained model as a FastAPI service
15. Final project — end-to-end model with training log, report, and demo

## Weekly Structure
Each lab = a Jupyter notebook + a short `REPORT.md` covering:
- The problem and the dataset
- The model architecture and why
- Training curves and final metrics
- Ablations or comparisons (where applicable)
- One lesson learned and one failure

## Assessment

| Component | Weight |
| :--- | :---: |
| Weekly lab reports (15) | 60% |
| Code quality and reproducibility (seeds, requirements) | 20% |
| Final project — model + report + demo | 20% |

## Deliverable Layout
deep-learning-lab/
├── reports/
│ ├── lab-01-backprop-numpy.md
│ ├── lab-02-pytorch-comparison.md
│ └── ...
├── notebooks/
│ ├── lab-01-backprop-numpy.ipynb
│ └── ...
├── requirements.txt
└── final-project/
├── README.md
├── train.py
├── infer.py
└── report.pdf

text

## Reproducibility Rules

- Every notebook must set random seeds (Python, NumPy, PyTorch).
- `requirements.txt` must pin versions.
- Training runs must log to Weights & Biases or a CSV.
- Any reported number must be reproducible with one command.
