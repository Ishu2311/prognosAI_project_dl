# 🔧 PrognosAI: AI-Driven Predictive Maintenance System Using Time-Series Sensor Data

## 🎯 Project Objective

Design and develop an AI-based predictive maintenance system to estimate the Remaining Useful Life (RUL) of industrial machinery using multivariate time-series sensor data. This prototype uses the NASA CMAPSS dataset and is adaptable across domains like turbines, pumps, and motors. The goal is to enable timely maintenance decisions, minimize unplanned downtime, and optimize asset utilization with deep learning models such as LSTM for sequential pattern recognition and failure prediction.

---

## 🗂️ Project Workflow

1. **Data Ingestion**  
   - Load and preprocess the CMAPSS sensor dataset (cycle-wise engine data).

2. **Feature Engineering**  
   - Create rolling window sequences and compute Remaining Useful Life (RUL) targets.

3. **Model Training**  
   - Train a time-series model (e.g., LSTM or GRU) to predict RUL from sensor sequences.

4. **Model Evaluation**  
   - Evaluate model performance using RMSE and compare predicted RUL vs actual RUL.

5. **Risk Thresholding**  
   - Define thresholds to trigger maintenance alerts based on predicted RUL.

6. **Visualization & Output**  
   - Present results through charts and dashboards showing RUL trends and alert zones.

## 🛠️ Tech Stack

- **Python** – Core programming language  
- **Pandas, NumPy** – Data processing  
- **Matplotlib, Seaborn** – Visualization  
- **TensorFlow / Keras** – LSTM model training  
- **Scikit-learn** – Metrics & preprocessing  
- **Streamlit / Flask** – Dashboard or API interface  
- **Docker** – Optional deployment  
- **NASA CMAPSS Dataset** – Source data  

---


## 🚀 Quick Start: prognosAI Project

Follow these simple steps to set up and test the project:

1. **Clone the Repository**
   - Open your terminal or command prompt.
   - Run the command below to clone the project repository:
     ```
     git clone https://github.com/prognosAI-Infosys-Intern-project/prognosAI-Intern-project.git
     ```
   - Change directory to the project folder:
     ```
     cd prognosAI-Intern-project/Project
     ```

2. **Create and Activate Python Virtual Environment**
   - Run the following command to create a virtual environment named `venv`:
     ```
     python -m venv venv
     ```
   - Activate the virtual environment:
     - On Linux/macOS:
       ```
       source venv/bin/activate
       ```
     - On Windows:
       ```
       venv\Scripts\activate
       ```

3. **Install Required Dependencies**
   - Install the required Python packages using:
     ```
     pip install -r requirements.txt
     ```

4. **Run Data Preprocessing**
   - Prepare the datasets and feature sequences by running:
     ```
     python data_preprocessing.py
     ```

5. **Train the Model**
   - Train the predictive maintenance model by executing:
     ```
     python train_model.py
     ```

6. **Start Streamlit Dashboard**
   - Launch the interactive web dashboard for predictions and alerts:
     ```
     streamlit run app.py
     ```

7. **Upload Test Data**
   - Use the Streamlit app interface to upload `sequence` and `metadata` files located in:
     ```
     processed_data/test
     ```
   - View model predictions and alert zones on the dashboard.
