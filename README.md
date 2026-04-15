# 📌 Inter-Class Cross-Domain Image Retrieval

An inter-class cross-domain image retrieval model that learns a shared embedding space using deep metric learning to retrieve semantically similar images across different domains while distinguishing between different classes.

Dataset-https://www.hemanthdv.org/officeHomeDataset.html

---

## 🚀 Overview

This project focuses on retrieving visually and semantically similar images across different domains such as:

- 🎨 Art  
- ✂️ Clipart  
- 🛍️ Product  
- 📷 Real World  

The model aligns representations from different domains into a **shared embedding space**, enabling robust retrieval despite domain shifts.

---

## 🧠 Key Features

- Cross-domain representation learning  
- Metric learning with triplet-based sampling  
- Domain adaptation using GRL (Gradient Reversal Layer)  
- Cosine similarity-based retrieval  
- Evaluation using **Recall@K** and **mAP**  
- t-SNE visualization of embeddings  
- Automated training + evaluation pipeline  

---

## 📂 Folder Structure

```
|- Dataset
|- config.py
|- create_csv.py
|- dataset_index.csv
|- dataset.py
|- EDA.py
|- inference.py
|- losses.py
|- metrics.py
|- model.py
|- plot_config_scores.py
|- requirements.txt
|- run_pipeline.bat
|- test.py
|- train.py
|- utils.py
|- val.py
```

---

## ⚙️ Installation

### 1. Clone the repository
```bash
git clone <your-repo-link>
cd <repo-name>
```

### 2. Install dependencies
```bash
pip install -r requirements.txt
```

---

## 📦 Requirements

- torch  
- torchvision  
- numpy  
- pandas  
- matplotlib  
- tqdm  
- transformers  
- scikit-learn  
- Pillow  

---

## ▶️ How to Run

Run the full pipeline:

```bash
.\run_pipeline.bat
```

This will:
- Create virtual environment  
- Install dependencies  
- Run EDA  
- Train all configurations  
- Select best model  
- Evaluate on test set  
- Generate retrieval samples  

---

## 🧩 Pipeline Overview

1. Dataset Preparation  
2. EDA  
3. Training  
4. Validation  
5. Testing  
6. Inference  

---

## 📊 Outputs

- outputs/checkpoints/ → Best models  
- outputs/logs/ → Training logs  
- outputs/reports/ → Metrics & reports  
- outputs/embeddings/ → Saved embeddings  
- outputs/samples/ → Retrieval examples  
- outputs/eda/ → Dataset analysis  

---

## 📈 Evaluation Metrics

- Recall@K  
- mAP  
- Cosine Similarity  

---

## 🏗️ Model Architecture

- Pretrained backbone  
- Projection head  
- Class classifier  
- Domain classifier + GRL  

---
