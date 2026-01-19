Network Traffic Classification App
This Streamlit application allows you to classify network traffic patterns using different machine learning models.

Features
Multiple model selection (Random Forest, Decision Tree, Naive Bayes, KNN)
Interactive data upload and preview
Real-time classification
Visualization of results
Model information and descriptions
Requirements
Python 3.7+
Required packages listed in requirements.txt
Installation
Clone this repository:
git clone <repository-url>
cd network-traffic-classification
Create a virtual environment (optional but recommended):
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
Install the required packages:
pip install -r requirements.txt
Usage
Run the Streamlit app:
streamlit run app.py
Open your web browser and navigate to the provided URL (typically http://localhost:8501)

Upload your network traffic data (CSV file)

Required columns: Length, Protocol, Source, Destination
Select a classification model from the sidebar

Click "Classify Traffic" to see the results

Data Format
Your CSV file should contain the following columns:

Length: Packet length
Protocol: Network protocol
Source: Source IP/address
Destination: Destination IP/address
Models Available
Random Forest

Best for complex patterns and handling large datasets
High accuracy and good generalization
Decision Tree

Simple and interpretable
Good for understanding decision rules
Naive Bayes

Fast and efficient
Works well with high-dimensional data
K-Nearest Neighbors

Good for pattern recognition
Works well with similar traffic patterns
