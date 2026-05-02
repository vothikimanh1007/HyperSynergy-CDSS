# 📂 GitHub Directory Structure: examples/biosnap_ddi_sota/

To allow the research community to easily reproduce your SOTA results, you should organize the example directory on GitHub as follows:

hypersynergy/

├── examples/

│ └── biosnap_ddi_sota/

│ ├── README.md <-- Specific instructions for this example

│ ├── requirements.txt <-- Auxiliary libraries (seaborn, sklearn)

│ ├── train_sota_ddi.py <-- Main code file (from your Canvas)

│ └── results/ <-- Directory for output images

│ ├── ddi_correlation.png

│ └── poincare_manifold.png

## 📄 File Content: examples/biosnap_ddi_sota/README.md

### 🌿 HyperSynergy: BIOSNAP DDI Benchmark (SOTA Best Practice)

This example demonstrates how to apply the **Manifold-Aware Transformer Gating (MATG)** model to predict drug-drug interactions (DDI) on the Stanford standard dataset (BIOSNAP).

#### 🚀 Key Results

- **Correlation Coefficient:** Achieved **~0.77** between the AI Alpha weights and the actual network degree.
- **Features:** Automatically identifies "Toxicity Architects" (key drugs causing toxicity) through Poincaré geometry.
- **Optimization Techniques:** Utilizes Topological Prior Loss and Dynamic Negative Sampling.

#### 🛠 How to Run

- Install the library: pip install hypersynergy==0.1.4
- Run the training script: python train_sota_ddi.py
- Check the biosnap_sota_analysis_results.csv file to view the hierarchical ranking of 1,514 drugs.

## 🧪 Requirements (requirements.txt)

torch>=2.0.0

pandas

numpy

matplotlib

seaborn

scikit-learn
