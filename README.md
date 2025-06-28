# 🌿 Ayurvedic Recommendation System

[![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue.svg)](https://www.python.org/downloads/)

🔮 A machine learning system that provides personalized Ayurvedic condition predictions and treatment recommendations based on user symptoms.

## ✨ Features

- **🩺 Symptom Analysis**: Multi-symptom selection with severity levels
- **🤖 Dual Models**: Decision Tree and Hierarchical Graph Convolutional Network (HeirGCN)
- **🔬 Disease Comparison**: Compare conditions to identify symptoms and treatments
- **📊 Interactive Interface**: Jupyter notebook with real-time visualizations
- **📈 Performance Insights**: Model comparison and accuracy metrics

## 🚀 Quick Start

1. **📦 Install Dependencies**
   ```bash
   pip install numpy pandas matplotlib seaborn torch torch-geometric scikit-learn ipywidgets
   ```

2. **▶️ Run the System**
   ```bash
   jupyter notebook ayurvedic_recsys.ipynb
   ```

3. **🎯 Use the Interface**
   - Select symptoms and severity level
   - Choose model (HeirGCN recommended)
   - Get predictions and treatment recommendations

## 📊 Performance

| Model | Accuracy | F1-Score |
|-------|----------|----------|
| Decision Tree | 78.5% | 0.76 |
| HeirGCN | 89.2% ⭐ | 0.87 ⭐ |

🏆 HeirGCN outperforms traditional ML by modeling complex symptom-disease relationships through graph neural networks.

## 📁 Project Structure

```
├── ayurvedic_recsys.ipynb    # 📓 Main notebook with complete system
└── README.md                 # 📖 This file
```


---

⚠️ **Note**: This system is for educational and research purposes only. Always consult qualified Ayurvedic practitioners for medical advice.
