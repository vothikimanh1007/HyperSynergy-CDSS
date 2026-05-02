# 🌿 HyperSynergy CDSS: Official User Guide

Welcome to the **HyperSynergy Clinical Decision Support System (CDSS)**!

This website acts as an intelligent assistant for Traditional Medicine (TM) practitioners and researchers. It uses a powerful AI (Graph Neural Network) to read traditional herbal formulas and predict if the combination of herbs will be safe, balanced, and effective.

You do **not** need to be a computer scientist or a master herbalist to use this tool. This guide will walk you through the interface and explain exactly how to interpret the AI's results.

## 🖥️ 1. Understanding the Interface (GUI)

The website is divided into three main sections:

- **The Left Panel (Build Prescription):** This is your workspace. Here, you will search for herbs from our 714-herb database and combine them into a digital "formula."
- **The Top Right Panel (Dashboard):** This is the AI's quick-glance summary. It gives you the overall Synergy Score, the Biological Distance, and a Formula Balance check.
- **The Bottom Right Panel (AI Role Assignments):** This detailed table explains _why_ the AI gave you that score. It breaks down every herb and reveals its specific job in the formula.

## 🛠️ 2. Step-by-Step: How to Use the App

### Step 1: Search and Add Herbs

- Go to the **Build Prescription** panel on the left.
- Click the search bar and type an herb's name (e.g., _Đương Quy_ or _Đại táo_).
- The system will automatically suggest herbs from the Vietnamese Pharmacopoeia as you type.
- Click the herb you want, or click the **blue "+" button** to add it to your "Current Formula" list.
- _Note: You must add at least_ **_two_** _herbs to run an analysis._

### Step 2: Run the AI

- Once your herbs are listed in the box, click the big blue **"Run Live PyTorch Analysis"** button.
- The website will send your formula across the internet to our cloud-based AI. The AI will do millions of mathematical calculations in just a few milliseconds!

### Step 3: Read the Executive Summary

- Look at the **Executive Summary & Recommendation** box. This is the "Doctor's Note."
- It will explicitly tell you if the formula is highly viable, structurally incomplete, or at a high risk of clinical conflict.

## 📊 3. How to Understand the Results (For Beginners)

The AI provides several metrics. Here is what they mean in plain English:

### 🟢 Overall Synergy Probability

This is the ultimate safety and effectiveness score.

- **80% - 100% (Green):** Excellent. The herbs work perfectly together.
- **50% - 79% (Blue):** Moderate. They won't hurt, but the combination could be stronger.
- **Below 50% (Orange/Red):** Poor. These herbs clash or do not help each other. High risk of side effects.

### 📏 Biological Distance (Poincaré Metric)

Imagine the AI has a 3D map of every herb's biological effects.

- If the gauge is **Green (Tight)**, the herbs are standing right next to each other on the map, meaning they target similar diseases and pathways.
- If the gauge is **Red (Far)**, the herbs are on opposite sides of the map, meaning they are likely pulling the body in two conflicting directions.

### ⚖️ Formula Balance Composition

Ancient traditional medicine relies on the _Quân-Thần-Tá-Sứ_ (Sovereign-Minister-Assistant-Courier) rule. A safe formula must be balanced.

- **Main Healer (Architect):** The formula _must_ have an aggressive herb to fight the disease.
- **Protector (Buffer):** The formula _must_ have a gentle herb (like Honey or Jujube/Đại táo) to protect the stomach from the harsh Main Healer.
- _If the AI gives you a red "X" here, it means you forgot a crucial piece of the puzzle!_

### 📋 The XAI Table (Role Assignments)

XAI stands for "Explainable AI." This table proves the AI isn't just guessing.

- **AI Importance (![](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAA8AAAAfCAYAAAA4AJfRAAAB00lEQVR4AeyRMUgzQRCF79b88JOIghDUJsmFYCGSwjQWQRAEixSChSJpBLXUTrC1sdBOLbRUG9FCbMRgKQiCpYioCbkjqEQjaqFCuJzfXCEXBSFY2CTsy8y8eTM7N6u0X/zqxTUur74wz8KCwWBjOBxuj0Qi/z10lft1YQ2hUGiYgku/33+GcsdxnEeabMO1EVedz+JoNNqMaEvX9TUUU6ZpGqZpJm3bjhMnwYZMg9XQLYG0W5xIJP4hWiQxBCby+XwG6wCtUChkuT0D+gOBQNIwjFb8DnLHbnGpVBonmIQ8pMk+vvdIkwsInXw36GO6K6bKKxkXYoykppTa5aY38b1AXJAYXS9Ig1ViR+FEcDrBa6VSOcV+O2hehKTJAP6RZVnnEivG9OE0gAeSN9ifzgEXLCOQT9EUwR3BPSjS9R379egQMp1G86L3sxSB3LaJIE5xF/bz8BwG2IFIgVfy4Vgs1sSbj7L1uGzbYfR5kkssLCNikuvYa7gVblu0LCtF4RxxT7lc3sNPw5tSLG/5xupnIFoQTJOcxe+CS/HmJ3A2DRbg2nw+3wj8YC6Xe3aLSboH4TuJW4H4Lun5g3vKZrNFKBtoVcVC1IJ6cS3bQvt3C/sAAAD///EWsEEAAAAGSURBVAMAVqrjP0/ebrQAAAAASUVORK5CYII=) Weight):** The AI scores every herb from 0.0 to 1.0. A high score (like 0.88) means the AI considers this herb the "Anchor" of the whole formula.
- **Clinical Role:** Based on that score, the AI automatically categorizes the herb:
  - 🔴 **Architect:** The boss. Directs the healing.
  - 🔵 **Bridge:** The transporter. Moves the medicine to the right organ.
  - 🟢 **Buffer:** The bodyguard. Protects the patient from side effects.

## 💡 Pro-Tip for your First Try

If you want to see a **Perfect Synergy** score, try adding these three herbs together and click Run:

- **Đương Quy** (The Architect - builds blood)
- **Xuyên khung** (The Bridge - moves blood)
- **Đại táo** (The Buffer - protects the stomach)
