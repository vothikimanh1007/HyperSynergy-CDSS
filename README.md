# HyperSynergy CDSS: Clinical Decision Support System 🌿

The **HyperSynergy Clinical Decision Support System (CDSS)** is an interactive, AI-driven web application designed to predict the pharmacological synergy of traditional herbal formulations. This tool bridges centuries of Vietnamese Traditional Medicine (VTM) and Traditional Chinese Medicine (TCM) with modern geometric deep learning.

Access the live web application here: [HyperSynergy CDSS](https://vothikimanh1007.github.io/HyperSynergy-CDSS/)

## 🔬 Core AI Architecture

This platform serves as the clinical interface for the **Manifold-Aware Transformer Gating (MATG)** neural network. Trained on the comprehensive **DoTatLoi-714 benchmark dataset**, the model maps the structural relationships of herbs into a hyperbolic space (Poincaré ball) to calculate synergy and identify potential clinical conflicts.

### Key Features

- **Live Synergy Probability:** Real-time calculation of formulation viability using the remote PyTorch API.
- **Biological Distance (Poincaré Metric):** Visualizes the topological distance between herbs; tighter distances imply stronger structural synergy.
- **Formula Balance Checker:** Automatically analyzes the prescription to ensure the presence of critical traditional roles, such as the Main Healer (Architect/Sovereign) and Protector (Buffer/Assistant).
- **Explainable AI (XAI):** Unpacks the AI's internal attention weights (![](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAA8AAAAfCAYAAAA4AJfRAAAB00lEQVR4AeyRMUgzQRCF79b88JOIghDUJsmFYCGSwjQWQRAEixSChSJpBLXUTrC1sdBOLbRUG9FCbMRgKQiCpYioCbkjqEQjaqFCuJzfXCEXBSFY2CTsy8y8eTM7N6u0X/zqxTUur74wz8KCwWBjOBxuj0Qi/z10lft1YQ2hUGiYgku/33+GcsdxnEeabMO1EVedz+JoNNqMaEvX9TUUU6ZpGqZpJm3bjhMnwYZMg9XQLYG0W5xIJP4hWiQxBCby+XwG6wCtUChkuT0D+gOBQNIwjFb8DnLHbnGpVBonmIQ8pMk+vvdIkwsInXw36GO6K6bKKxkXYoykppTa5aY38b1AXJAYXS9Ig1ViR+FEcDrBa6VSOcV+O2hehKTJAP6RZVnnEivG9OE0gAeSN9ifzgEXLCOQT9EUwR3BPSjS9R379egQMp1G86L3sxSB3LaJIE5xF/bz8BwG2IFIgVfy4Vgs1sSbj7L1uGzbYfR5kkssLCNikuvYa7gVblu0LCtF4RxxT7lc3sNPw5tSLG/5xupnIFoQTJOcxe+CS/HmJ3A2DRbg2nw+3wj8YC6Xe3aLSboH4TuJW4H4Lun5g3vKZrNFKBtoVcVC1IJ6cS3bQvt3C/sAAAD///EWsEEAAAAGSURBVAMAVqrjP0/ebrQAAAAASUVORK5CYII=)) to assign ancient _Quân-Thần-Tá-Sứ_ hierarchical roles with plain-English clinical explanations.

## 🛠️ Deployment Structure (Headless API)

This project utilizes a modern, serverless front-end architecture communicating with a dedicated AI microservice:

- **Frontend (This Repository):** A lightweight, static HTML/JS/TailwindCSS application hosted on GitHub Pages. It utilizes a pre-compiled database.json for lightning-fast autocomplete and global weight calibration.
- **Backend API (Hugging Face Spaces):** A FastAPI server hosting the Proposed_MATG_Ours_v82_Final_MATG_400_Epochs_Best.pth PyTorch weights. It receives herb queries, executes the MATG tensor math, and returns the XAI payload.

## 🚀 How to Use

- **Search & Add Herbs:** Use the search bar to find herbs from the 714-herb database (e.g., _Đương Quy_, _Đại táo_).
- **Run AI Analysis:** Click the blue button to send your custom formulation to the PyTorch server.
- **Review Recommendations:** The CDSS will generate an Executive Summary detailing the formula's safety, structural completeness, and clinical viability.

## 🎓 Academic Context

This application is the culmination of a Ph.D. research project focusing on Macro-to-Micro Geometric Learning.

**Lead Researcher:** Vo Thi Kim Anh

- _Ph.D. Candidate_, VSB - Technical University of Ostrava, Czech Republic
- _Researcher_, Ton Duc Thang University, Vietnam

**Contact:** [vothikimanh@tdtu.edu.vn](mailto:vothikimanh@tdtu.edu.vn) | [thi.kim.anh.vo.st@vsb.cz](mailto:thi.kim.anh.vo.st@vsb.cz)
