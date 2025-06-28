# Ayurveda-Based Medical Recommendation System

## Overview
This repository contains the implementation of an **Ayurveda-Based Medical Recommendation System** developed as a mini-project for the course CSE300/INT300/ICT300 at SASTRA Deemed to be University. The system leverages a **Hierarchical Graph Convolutional Network (HierGCN)** with Top-K Pooling and a **Decision Tree Classifier** to recommend treatments for Ayurvedic diseases based on symptoms and their severity. The project uses a synthetic Ayurvedic dataset and includes an interactive user interface built with Jupyter Notebook and ipywidgets.

## Authors
- Akash Kumar P R
- Kenneth Aidan I
- Thejes Ram S

## Repository Contents
- **ayurvedic_recsys_report.pdf**: The project report detailing the methodology, implementation, results, and conclusions of the Ayurveda-Based Medical Recommendation System.
- **ayurvedic_recsys.ipynb**: The Jupyter Notebook containing the source code for the recommendation system, including data generation, preprocessing, model training (HierGCN and Decision Tree), and the interactive user interface.

## Project Description
The system aims to automate Ayurvedic disease diagnosis and treatment recommendation by modeling disease-symptom relationships using graph-based and traditional machine learning approaches. Key features include:
- **Dataset**: A synthetic dataset with 10,000 samples, including 150 Ayurvedic diseases, 159 symptoms, severity levels (Mild, Moderate, Severe), and 2-5 treatments per disease.
- **Models**:
  - **HierGCN**: A Hierarchical Graph Convolutional Network with Top-K Pooling to capture complex disease-symptom relationships.
  - **Decision Tree**: A baseline classifier using scikit-learn for comparison.
- **User Interface**: An interactive UI built with ipywidgets in Jupyter Notebook, allowing users to input symptoms and severity to receive treatment recommendations.
- **Performance**:
  - HierGCN: ~95% accuracy, ~0.93 F1-Score.
  - Decision Tree: ~90% accuracy, ~0.89 F1-Score.

## Requirements
### Hardware
- PC with 250GB storage
- Intel i3 processor or equivalent
- 4GB RAM
- Optional: GPU for faster GNN training

### Software
- Python 3.8+
- Libraries: `PyTorch`, `torch_geometric`, `pandas`, `numpy`, `scikit-learn`, `matplotlib`, `seaborn`, `networkx`, `ipywidgets`
- Jupyter Notebook for development and visualization

## Installation
1. Clone the repository:
   ```bash
   git clone <repository-url>
   cd <repository-directory>
   ```
2. Install the required Python libraries:
   ```bash
   pip install torch torch-geometric pandas numpy scikit-learn matplotlib seaborn networkx ipywidgets
   ```
3. Launch Jupyter Notebook:
   ```bash
   jupyter notebook
   ```
4. Open `ayurvedic_recsys.ipynb` to run the code and interact with the system.

## Usage
1. Open `ayurvedic_recsys.ipynb` in Jupyter Notebook.
2. Run the cells sequentially to:
   - Generate the synthetic Ayurvedic dataset.
   - Preprocess the data and construct a bipartite graph.
   - Train and evaluate the HierGCN and Decision Tree models.
   - Launch the interactive UI to input symptoms and severity for treatment recommendations.
3. Use the multi-select widget to choose symptoms, select severity, and click the prediction button to view results.

## Project Structure
- **Data Generation**: Creates a synthetic dataset with probabilistic symptom-disease mappings.
- **Preprocessing**: Encodes symptoms (one-hot), severity (label encoding), and constructs a bipartite graph.
- **HierGCN**: Implements a two-layer GCN with Top-K Pooling, trained with Adam optimizer and cross-entropy loss.
- **Decision Tree**: Uses scikit-learn’s DecisionTreeClassifier with default settings.
- **UI**: Built with ipywidgets for symptom selection, severity input, and visualization of results.
- **Visualization**: Displays bipartite graph and performance metrics (accuracy, F1-score, precision, recall, confusion matrix).

## Results
- **HierGCN**: Outperforms the Decision Tree due to its ability to model complex graph-based relationships, achieving ~95% accuracy and ~0.93 F1-Score.
- **Decision Tree**: Simpler model with ~90% accuracy and ~0.89 F1-Score, less effective for interconnected data.
- **Limitations**: Reliance on synthetic data and high computational requirements for HierGCN.

## Future Directions
- Incorporate real-world Ayurvedic data.
- Enhance the model with attention mechanisms and temporal graph modeling.
- Develop a mobile app for broader accessibility.
- Include personalized treatment plans and dietary recommendations.

## Acknowledgments
- Project Supervisor: Mr. Eashwar K B, Assistant Professor - II, Department of Computer Science and Engineering, Srinivasa Ramanujan Centre.
- Project Review Panel: Dr. Sreedevi B and Dr. Venkateswari P.
- Project Coordinator: Dr. Vaishnavi D, Assistant Professor-II, Department of Computer Science and Engineering, Srinivasa Ramanujan Centre.
- SASTRA Deemed to be University for providing infrastructure and support.

## License
This project is for academic purposes and is not licensed for commercial use. Please contact the authors for any tranquility inquiries.
