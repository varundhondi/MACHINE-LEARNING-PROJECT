# 🚗 Carpooling Optimization System using Machine Learning

[cite_start]This project presents an intelligent carpooling optimization system designed to efficiently match drivers and passengers, implement a dynamic pricing model, and ensure equitable cost distribution[cite: 13, 15]. [cite_start]By leveraging a suite of machine learning algorithms and optimization techniques, the system aims to provide a sustainable, cost-effective, and efficient transportation solution[cite: 13, 206].

[cite_start]This system was developed as part of the CSE4036 Machine Learning course project at Vellore Institute of Technology, Chennai[cite: 1, 2, 3].

---
## 🎯 Problem Statement

[cite_start]The primary goal is to develop a comprehensive carpooling system that tackles several key challenges in ride-sharing[cite: 18]:

* [cite_start]**User Matching Optimization**: Efficiently pair drivers with passengers based on spatial-temporal constraints, user preferences, and vehicle capacity[cite: 19, 20, 21, 22].
* [cite_start]**Dynamic Pricing System**: Implement a fair and transparent pricing model that adjusts in real-time based on variables like fuel prices, trip distance, passenger count, and peak hours[cite: 24, 25, 30].
* [cite_start]**Equitable Cost Distribution**: Create a framework for the fair division of travel expenses among passengers while ensuring adequate compensation for the driver[cite: 31, 32, 34].
* [cite_start]**System Efficiency**: Minimize waiting times and optimize route selection to balance overall system efficiency with individual user preferences[cite: 35, 36, 37, 38].

---
## ✨ Features

The system integrates several advanced ML techniques to deliver a robust solution:

* [cite_start]**User Clustering**: Groups users based on location and time using **K-Means** for spatial-temporal grouping and **Hierarchical Clustering** for multi-level segmentation[cite: 77, 78, 79, 237].
* [cite_start]**Matching Optimization**: Employs **Linear Programming** (via `scipy.optimize.linear_sum_assignment`) to determine the most cost-effective driver-passenger pairings[cite: 81, 82, 123].
* [cite_start]**Dynamic Pricing Model**: Utilizes **Gaussian Mixture Models (GMM)** to create price clusters that adapt to real-time variables, ensuring a dynamic and fair pricing structure[cite: 85, 86, 128].
* [cite_start]**Success Prediction**: A predictive module powered by an **XGBoost Classifier** predicts the likelihood of a successful match, helping to optimize system-wide pairings[cite: 89, 90, 252].
* [cite_start]**Data Visualization**: Includes a range of visualizations using Matplotlib and Seaborn, such as heatmaps of cluster density, hierarchical dendrograms, and cost distribution plots, to analyze system performance[cite: 161, 314].

---
## 🏗️ System Architecture

The system is built on a modular architecture where each component handles a specific optimization task. [cite_start]These components are designed to be integrated via REST APIs for a real-time data processing pipeline[cite: 93, 94, 95].

1.  [cite_start]**User Clustering Module** [cite: 77]
2.  [cite_start]**Matching Optimization Engine** [cite: 81]
3.  [cite_start]**Dynamic Pricing System** [cite: 85]
4.  [cite_start]**Predictive Analytics Module** [cite: 89]



---
## 🛠️ Setup and Installation

To get this project up and running on your local machine, follow these steps.

### Prerequisites
* Python 3.x
* Jupyter Notebook or JupyterLab
* pip (Python package installer)

### Installation
1.  **Clone the repository:**
    ```sh
    git clone [https://github.com/your-username/carpooling-optimization.git](https://github.com/your-username/carpooling-optimization.git)
    cd carpooling-optimization
    ```
2.  **Create a `requirements.txt` file** with the following content:
    ```text
    pandas
    scikit-learn
    xgboost
    matplotlib
    seaborn
    scipy
    numpy
    ```
3.  **Install the required dependencies:**
    It is recommended to use a virtual environment.
    ```sh
    pip install -r requirements.txt
    ```

---
## 🚀 Usage

1.  Place the datasets (`carpooling_dataset.csv` and `daily_petrol_prices.csv`) in the root directory of the project.
2.  Launch Jupyter Notebook:
    ```sh
    jupyter notebook ML_Jcomp.ipynb
    ```
3.  Run the cells in the notebook sequentially to perform data preprocessing, clustering, matching, and analysis.

---
## 📊 Results and Analysis

The implemented system demonstrated significant improvements in carpooling efficiency and user satisfaction.

| Metric | Result |
| :--- | :--- |
| **Clustering Performance** | |
| Average Silhouette Score | [cite_start]0.68 [cite: 134] |
| **Matching Efficiency** | |
| Success Rate | [cite_start]85% [cite: 138] |
| Average User Satisfaction | [cite_start]4.2 / 5 [cite: 140] |
| **Pricing Optimization** | |
| Average Cost Reduction per User| [cite_start]23% [cite: 142] |
| Price Fairness Rating | [cite_start]4.1 / 5 [cite: 143] |

### Visualizations

* [cite_start]**Cluster Summary Heatmap**: Shows the distribution of drivers and passengers across different clusters[cite: 163].
* [cite_start]**Hierarchical Clustering Dendrogram**: Visualizes the multi-level user segments created by the algorithm[cite: 121].
* [cite_start]**Cost Distribution Histogram**: Displays the frequency of different cost-per-passenger values, demonstrating the model's pricing fairness[cite: 164].



---
## 🔮 Future Work

Based on the analysis, several areas for future improvement have been identified:

* [cite_start]**Real-time Data Integration**: Incorporate live traffic data to enhance route optimization[cite: 151].
* [cite_start]**Scalability Enhancements**: Explore heuristic or metaheuristic algorithms (e.g., Genetic Algorithms) to replace linear programming for better performance on larger datasets[cite: 276, 340].
* [cite_start]**Model Tuning**: Perform comprehensive hyperparameter tuning for clustering and classification models to improve accuracy[cite: 338].
* [cite_start]**User Feedback Loop**: Implement an A/B testing framework and enhance the user feedback integration for continuous model improvement[cite: 156, 157].

---
## 🧑‍💻 Contributors

* [cite_start]**Dhondi Varun** - `22MIA1200` [cite: 6, 201]
* [cite_start]**Kashish Gidwani** - `22MIA1117` [cite: 7, 202]
