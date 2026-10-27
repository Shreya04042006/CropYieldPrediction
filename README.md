🌾 Crop Yield Prediction & Harvest Analysis Engine
An interactive, data-driven machine learning application and executive web deck designed to estimate agricultural output based on historical climate, soil, and land parameters.

📌 Table of Contents
Overview
Key Features
Tech Stack
Dataset Information
Workflow & Pipeline
Installation & Setup
Project Structure
Usage
Future Scope
📖 Overview
The Crop Yield Prediction Engine analyzes multi-year historical agricultural records across various crop varieties to predict harvest performance and land efficiency. By processing key variables such as temperature, seasonal rainfall, land area, and soil moisture levels, this system enables agricultural managers and advisors to make informed, data-backed decisions.

✨ Key Features
📊 Interactive Web Presentation Deck: Built with 3D Three.js visual elements, animated GSAP slide transitions, and dynamic Chart.js figures.
🧮 Live Yield Estimator: Interactive simulation tool allowing real-time adjustment of land area, temperature, and moisture levels to project crop tonnage.
🧹 Robust Machine Learning Pipeline: Integrated preprocessing via Column Transformers, StandardScaler, and One-Hot Encoding.
📈 Multi-Model Regression Suite: Evaluates multiple machine learning algorithms for precise yield forecasting.
🛠 Tech Stack
Programming Language
Python
Data Processing & Analytics
Pandas – Dataframe manipulation and dataset processing
NumPy – Linear algebra and numerical computing
Data Visualization
Matplotlib & Seaborn – Exploratory Data Analysis & visual plotting
Chart.js – Interactive frontend charting
Machine Learning (Scikit-Learn)
Preprocessing: ColumnTransformer, Pipeline, OneHotEncoder, StandardScaler
Regression Algorithms:
Linear Regression
Lasso Regression
Ridge Regression
Decision Tree Regressor
K-Nearest Neighbors (KNN) Regressor
Model Serialization
Pickle – Exporting and loading trained model & preprocessor pipelines
Web Framework & Frontend
Flask – Python web framework
HTML5 / CSS3 / JavaScript
Development Tools
Jupyter Notebook (Prototyping & EDA)
VS Code (Application Development)
📂 Dataset Information
Records: 49,784 cleaned entries
Timeframe: 1990 – 2014 (24 years of historical agricultural records)
Crops: 80 unique crop varieties (e.g., Rice, Banana, Arecanut, Kharif Pulses, Wheat)
Data Quality: 0 null values, verified duplicate-free, normalized numerical inputs.
⚙️ Workflow & Pipeline
Data Cleaning: Remove statistical outliers, handle duplicates, and audit missing parameters.
Feature Engineering: Group region, seasonal climate, and crop varieties into standardized feature sets.
Preprocessing: Apply One-Hot Encoding to categorical variables and StandardScaler to continuous numerical metrics.
Model Training & Selection: Train multiple regression models and measure error metrics (RMSE, 
R
2
 Score).
Deployment: Save preprocessor and model via Pickle; serve predictions interactively using Flask and dynamic Web UI.
🚀 Installation & Setup
Prerequisites
Python 3.8 or higher installed on your system.
1. Clone the Repository
git clone https://github.com/your-username/crop-yield-prediction.git
cd crop-yield-prediction
2. Create a Virtual Environment
# On Windows
python -m venv venv
venv\Scripts\activate

# On macOS/Linux
python3 -m venv venv
source venv/bin/activate
3. Install Dependencies
pip install -r requirements.txt
4. Run the Application
python app.py
Open your browser and navigate to http://127.0.0.1:5000/.

📁 Project Structure
├── data/
│   └── yield_df.csv            # Cleaned Crop Yield Dataset
├── notebooks/
│   └── yield_analysis.ipynb    # Data Cleaning, EDA & ML Model Benchmarking
├── models/
│   ├── model.pkl               # Trained Machine Learning Model
│   └── preprocessor.pkl        # Fitted Preprocessing Pipeline
├── static/
│   ├── css/                    # Stylesheets
│   └── js/                     # Three.js & Animation Scripts
├── templates/
│   └── index.html              # Presentation Deck & Yield Calculator
├── app.py                      # Flask Application Server
├── requirements.txt            # Python Dependencies
└── README.md                   # Project Documentation
🔮 Future Scope
🌤️ Live Weather API Integration: Automatically fetch current temperature and real-time precipitation metrics.
🧪 Soil NPK Quality Integration: Incorporate Nitrogen, Phosphorus, and Potassium metrics for refined yield predictions.
📱 Mobile Application: Expand responsive UI into a dedicated mobile application for field workers.
🤝 Contributing
Contributions, issues, and feature requests are welcome! Feel free to check the issues page.

📝 License
Distributed under the MIT License. See LICENSE for more information.

