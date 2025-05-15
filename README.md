# 🧠 ID3 Decision Tree from Scratch with Laptop Dataset

This repository contains a clean and educational implementation of the **ID3 (Iterative Dichotomiser 3)** decision tree algorithm using Python. The project walks through all key steps, from entropy calculation to prediction, and includes visualization using Graphviz.

## 📑 Table of Contents
- [Overview](#overview)
- [Dataset](#dataset)
- [Algorithm: ID3](#algorithm-id3)
- [Project Structure](#project-structure)
- [Installation](#installation)
- [Usage](#usage)
- [Visualization](#visualization)
- [Results](#results)
- [References](#references)

## 📌 Overview
The goal of this project is to demonstrate how a decision tree works internally by implementing the **ID3 algorithm** from scratch and applying it to a real-world dataset — a custom **laptop dataset**. We predict a target label (e.g., laptop purchase recommendation or performance level) based on categorical features like processor type, RAM size, brand, etc.

## 📦 Dataset
A custom dataset containing features about individuals and whether they bought a laptop:

| Age   | Income | Student | Credit_rating | Buy_Laptop |
|-------|--------|---------|---------------|------------|
| <=30  | High   | No      | Fair          | No         |
| <=30  | High   | No      | Excellent     | No         |
| 31-40 | High   | No      | Fair          | Yes        |
| >40   | Medium | No      | Fair          | Yes        |
| >40   | Low    | Yes     | Fair          | Yes        |
| >40   | Low    | Yes     | Excellent     | No         |
| 31-40 | Low    | Yes     | Excellent     | Yes        |
| <=30  | Medium | No      | Fair          | No         |
| <=30  | Low    | Yes     | Fair          | Yes        |
| >40   | Medium | Yes     | Fair          | Yes        |
| <=30  | Medium | Yes     | Excellent     | Yes        |
| 31-40 | Medium | No      | Excellent     | Yes        |
| 31-40 | High   | Yes     | Fair          | Yes        |
| >40   | Medium | No      | Excellent     | No         |

## 🧮 Algorithm: ID3
**ID3** builds a decision tree by recursively selecting the attribute that yields the **highest Information Gain**, calculated using **Entropy**. It stops when:
- All examples belong to the same class, or
- No more attributes are left to split, or
- The dataset becomes empty.

## 📁 Project Structure
```
📦 id3-laptop
├── ID3.ipynb                # Jupyter Notebook with full code
├── id3_tree.png             # Output decision tree visualization
├── dataset.csv              # Custom laptop dataset
├── README.md                # Project documentation
```

## ⚙️ Installation
Clone the repo:
```bash
git clone https://github.com/Likith-2004/id3-laptop.git
cd id3-laptop
```

Install dependencies:
```bash
pip install pandas graphviz scikit-learn
```

(Optional) Install **Graphviz** for visualization:
- **Windows**: Download from [https://graphviz.org/download/](https://graphviz.org/download/)
- Add the Graphviz `bin` path (where `dot.exe` is) to your system's PATH.

## ▶️ Usage
Open the notebook:
```bash
jupyter notebook ID3.ipynb
```

Run all the steps in the following order:
1. Load Dataset
2. Define Entropy and Information Gain Functions
3. Build ID3 Tree
4. Make Predictions
5. Evaluate Accuracy
6. Visualize Tree

## 🌳 Visualization
The tree is visualized using **Graphviz**. Example output is saved as `id3_tree.png` or `id3_tree.pdf` when running locally.

## 📊 Results
- The ID3 tree correctly classifies most entries based on laptop specs.
- Achieved accuracy on test split: ~XX% (depends on your dataset).

## 📚 References
- [ID3 Algorithm - Wikipedia](https://en.wikipedia.org/wiki/ID3_algorithm)
- *Machine Learning* by Tom Mitchell
- [Graphviz Documentation](https://graphviz.org/documentation/)
- [Scikit-learn](https://scikit-learn.org/)

  
### 🙌 **Contributors**
#### [Likith V K](https://github.com/Likith-2004) under guidance of [Dr Agughasi Victor Ikechukwu](https://github.com/Victor-Ikechukwu) <br>
---

## 🧑‍💻 Author
Made with ❤️ by [Likith V K].  
Feel free to raise issues or contribute!
