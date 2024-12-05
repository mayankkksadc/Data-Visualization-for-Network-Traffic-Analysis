

---

# **Network Traffic Analysis and Visualization**

## **Overview**
This repository contains the code, datasets, and results from the project *Network Traffic Analysis and Visualization*. The primary goal is to analyze network traffic patterns, detect cyber-attacks, and visualize actionable insights using machine learning techniques and real-time simulation tools like Power BI. This project leverages the CICIDS 2017 dataset for anomaly detection and explores the impact of dimensionality reduction using Principal Component Analysis (PCA) on model performance and visualization clarity.

---

## **Table of Contents**
1. [Project Objective](#project-objective)
2. [Key Features](#key-features)
3. [Datasets Used](#datasets-used)
4. [Project Structure](#project-structure)
5. [Installation](#installation)
6. [Usage](#usage)
7. [Results and Visualizations](#results-and-visualizations)
8. [Future Work](#future-work)
9. [Contributors](#contributors)
10. [References](#references)

---

## **Project Objective**
The project aims to:
- Analyze network traffic patterns to detect anomalies and cyber-attacks.
- Utilize dimensionality reduction techniques like PCA to improve computational efficiency.
- Create interactive and real-time visualizations in Power BI for better understanding and decision-making in cybersecurity.

---

## **Key Features**
- **Data Preprocessing**: Cleaning, scaling, and encoding the CICIDS 2017 dataset.
- **Dimensionality Reduction**: Implementing PCA to simplify the dataset and optimize performance.
- **Machine Learning Models**: Training XGBoost, Random Forest, Decision Tree, and Logistic Regression for anomaly detection.
- **Real-Time Simulation**: Simulating network traffic and streaming predictions to Power BI dashboards.
- **Visualization**: Interactive feature importance analysis, attack distribution graphs, and protocol-wise comparisons.

---

## **Datasets Used**
- **CICIDS 2017 Dataset**: Includes network traffic data labeled with attack types and benign traffic.
- **Simulated Data**: Derived from the CICIDS 2017 dataset, this simulated data is used for real-time visualization in Power BI.

---

## **Project Structure**
```
📂 Project Repository
├── 📂 Data
│   ├── Data_Google_Drive_Link       # Simulated network traffic data Google Drive Link
├── 📂 Python Files
│   ├── DV_Project_Preprocessing.ipynb                      # Data cleaning, transformation, and scaling
│   ├── DV_Project_Model.ipynb                              # Training ML models with and without PCA
│   ├── Network_Traffic_Analysis_Visualization.ipynb        # Visualizing model results and feature importance
│   ├──Simulation_pca.ipynb                                 # Real-time simulation with PCA
│   ├── Simulation.ipynb                                    # Real-time simulation without PCA
├── 📂 Packages and Models
│   ├── labelencoded.pkl           # Label Encoder instance
│   ├── pca.pkl                    # PCA instance
│   ├── scaler_pca.pkl             # Standard Scaler for PCA data
│   ├── stdscaler.pkl              # Standard Scaler for non-PCA data
│   ├── xgb_model.model            # XGBoost model for non-PCA data
│   ├── xgb_pca.model              # XGBoost model for PCA data
├── demo_project.md                # YouTube link for project demo
├── powerbi_visualization.md      # Google Drive link for Power BI real-time visualization
├── Paper.pdf                      # Pdf about the project report/paper
├── README.md                      # Project description and setup guide
```

---

## **Installation**
1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/network-traffic-analysis.git
   cd network-traffic-analysis
   ```

2. Install required dependencies:
   ```bash
   pip install -r requirements.txt
   ```

3. Download and place the dataset (`*.csv`) in the `Data` folder (There are multiple dataset and run the preprocessing python file.

---

## **Usage**
1. **Preprocessing**: Run `DV_Project_Preprocessing.ipynb` to clean and prepare the data.
2. **Model Training**:
   - Train ML models using `DV_Project_Model.ipynb`.
   - Evaluate performance with and without PCA.
3. **Visualization**:
   - Generate plots using `Network_Traffic_Analysis_Visualization.ipynb`.
4. **Real-Time Simulation**:
   - Simulate traffic with PCA: `Simulation_pca.ipynb`.
   - Simulate traffic without PCA: `Simulation.ipynb`.
5. **Power BI**:
   - Stream predictions and create dashboards with the provided API setup.

---

## **Results and Visualizations**
- **XGBoost Model**: Achieved the highest accuracy for anomaly detection.
- **PCA Impact**: Reduced training time by 27% with minimal accuracy loss.
- **Interactive Dashboards**: Real-time streaming in Power BI enabled dynamic analysis of network traffic and attack types.

---

## **Future Work**
1. Explore advanced dimensionality reduction techniques like t-SNE and UMAP.
2. Investigate deep learning models for improved anomaly detection.
3. Enhance scalability for larger datasets using distributed frameworks.
4. Develop more interactive and user-friendly visualizations.

---

## **Contributors**
- **Mayank Kapadia** - Data preprocessing, modeling, and real-time visualization.
- **Andrew Dunton, Chelsea Jaculina, Albert Ong, David Thach** - Team members contributing to analysis and methodology.

---

## **References**
- [CICIDS 2017 Dataset](https://www.unb.ca/cic/datasets/ids-2017.html)
- Kapadia, M., Dunton, A., Jaculina, C., Ong, A., Thach, D. Data Visualization and Preprocessing for Network Traffic Analysis in Cybersecurity.(Refer the **Paper.pdf** File)

---
