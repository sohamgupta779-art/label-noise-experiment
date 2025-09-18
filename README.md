# Label Noise Experiment on SST-2 with DistilBERT

This project explores the effect of **label noise** in sentiment classification using the SST-2 dataset (from GLUE) and DistilBERT.  

We fine-tuned DistilBERT on clean labels, then repeated training with **10%** and **20% random label noise** to study how performance changes.

---

##  Summary

- Fine-tuned **DistilBERT** on the **SST-2 dataset (GLUE benchmark)**.  
- Simulated noisy datasets by flipping **10%** and **20%** of labels.  
- Compared performance on clean vs noisy training data.  
- Found that **validation accuracy decreases** as label noise increases.  
- Results are visualized in `results.png` and reproduced in code.

##  Results

| Setting        | Validation Accuracy |
|----------------|----------------------|
| Clean labels   | (fill with your acc_baseline) |
| 10% noise      | (fill with your acc_noisy_10) |
| 20% noise      | (fill with your acc_noisy_20) |

> Replace the placeholders with your actual accuracy values from the notebook.

<img src="result.png" width="400">

---

##  How to Run

1. Clone this repo:
   ```bash
   git clone https://github.com/YOUR_USERNAME/label-noise-experiment.git
   cd label-noise-experiment
Install dependencies:

pip install -r requirements.txt


Open and run the notebook:

jupyter notebook notebook.ipynb



As label noise increases, DistilBERT’s validation accuracy drops.

This experiment demonstrates why robust training methods (like MAE loss or noise-aware training) are valuable in research.

Author: SOHAM GUPTA

