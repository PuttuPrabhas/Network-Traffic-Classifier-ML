# Network Traffic Classification App

A Streamlit-based web application for classifying network traffic patterns using multiple machine learning models. The tool supports interactive data upload, real-time predictions, and visualization of classification outputs.

## Features

- Multiple model options:
  - Random Forest
  - Decision Tree
  - Naive Bayes
  - K-Nearest Neighbors
- Real-time classification and results visualization
- Interactive CSV data upload and preview
- Model descriptions and selection guidance
- Lightweight and easy-to-run UI powered by Streamlit

## Requirements

- Python 3.7+
- Dependencies listed in `requirements.txt`

## Installation

Clone the repository:
```
git clone <repository-url>
cd network-traffic-classification
```

(Optional but recommended) create and activate a virtual environment:
```
python -m venv venv
source venv/bin/activate    # On Windows: venv\Scripts\activate
```

Install required packages:
```
pip install -r requirements.txt
```

## Usage

Run the Streamlit application:
```
streamlit run app.py
```

Open your browser and navigate to the provided URL (typically `http://localhost:8501`).

Steps:

1. Upload a CSV file containing network traffic data
2. Select a model from the sidebar
3. Click **Classify Traffic** to generate predictions
4. View results and visualizations directly in the UI

## Data Format

Uploaded CSV files must include:

| Column | Description |
|--------|-------------|
| Length | Packet length |
| Protocol | Network protocol name/identifier |
| Source | Source IP or address |
| Destination | Destination IP or address |

## Models Available

### Random Forest
- Suitable for complex patterns and larger datasets
- High accuracy and strong generalization performance

### Decision Tree
- Interpretability and rule-based analysis
- Useful for understanding classification criteria

### Naive Bayes
- Fast and computationally efficient
- Performs well on high-dimensional feature spaces

### K-Nearest Neighbors (KNN)
- Effective for similarity-based pattern recognition
- Good for scenarios where similar traffic behaves similarly

## Project Structure (Example)

```
network-traffic-classification/
│
├── app.py
├── requirements.txt
├── models/
│   ├── random_forest.pkl
│   ├── decision_tree.pkl
│   ├── naive_bayes.pkl
│   └── knn.pkl
└── data/
    └── sample.csv
```

## Future Improvements

- Support for additional protocols and traffic metrics
- Model benchmarking dashboard
- Automated feature extraction from raw packet data
- Deployment as a Docker container or cloud-hosted service

## License

Add your preferred license here (MIT, Apache-2.0, etc.).
