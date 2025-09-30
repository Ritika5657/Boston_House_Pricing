## Boston House Pricing Prediction: Machine Learning Deployment Project

This project implements a **Multiple Linear Regression** model to predict median house values in Boston suburbs, packaged as a lightweight web application using **Flask** and structured for cloud deployment (using Docker/Gunicorn).

---

### ⚙️ Technologies and Tools

* **Model:** Scikit-learn (Linear Regression, Iterative Imputer)
* **API Framework:** **Flask**
* **Data Handling:** Pandas, NumPy
* **Deployment Tools:** Gunicorn, Docker (Containerization)
* **Environment Manager:** Conda
* **Version Control:** Git

### 🚀 Project Structure

The repository is organized to separate the model training process from the web application interface.
```
Boston_House_Pricing/
├── data/
│   └── HousingData.csv         # The raw dataset.
├── templates/
│   └── home.html               # Frontend template for the web form.
├── app.py                      # Main Flask application file (API endpoints).
├── Procfile                    # Deployment configuration for Gunicorn.
├── requirements.txt            # List of Python dependencies.
├── regression.pkl              # Pickled (serialized) Linear Regression model.
├── scaling.pkl                 # Pickled (serialized) Scaler object for feature transformation.
└── Linear Regression ML Implementation.ipynb # Main notebook for EDA, Training, and Model Serialization.
```
### 📋 Software and Tools Requirements

1.  **GitHub Account**
2.  **VS Code IDE** (or similar Python editor)
3.  **Git CLI**
4.  **Conda/Anaconda** or **Miniconda** (for environment management)

### 💻 Local Setup and Execution

To run this project locally, follow these steps:

#### 1. Create a New Conda Environment

Open your VS Code terminal and run the following commands to create and activate an isolated environment.

```bash
# Create the environment (Using Python 3.7 as specified in the original plan)
conda create -p venv python==3.7 -y

# Activate the environment (Use your actual path if 'conda activate venv' fails)
conda activate venv
```

#### 2. Install Dependencies
Install all required Python packages (Flask, scikit-learn, Gunicorn, etc.) using the requirements.txt file:

```Bash

(venv) $ pip install -r requirements.txt
```
#### 3. Run the Flask Application
Execute the main application file.

```Bash

(venv) $ python app.py
The application will usually run on http://127.0.0.1:5000/. Open this link in your browser to view the prediction form.
```
