# 💎 Diamond Price Prediction API

This project provides an API interface for predicting diamond prices using a machine learning model trained on a comprehensive dataset of diamond features. It includes data cleaning, model training, serialization, and an API for querying predictions or filtered data.

---

## 🚀 Features

- **Data Handling**: Preprocessing includes handling missing values and encoding categorical variables like cut, color, and clarity.
- **Model Training**: Built with regression algorithms (e.g., Linear Regression or Random Forest) using scikit-learn.
- **Model Persistence**: The trained model is saved with `pickle` for reuse in the API.
- **API Endpoints**: Access training data, test data, predictions, and filtered results.
- **Interactive Querying**: Integrates with [Gamma.app](https://gamma.app) for dynamic exploration.

---

## 📦 Tech Stack

- **Python** – Core programming language
- **Pandas** – Data manipulation
- **Scikit-learn** – Machine learning
- **Pickle** – Model serialization
- **Flask** – Web framework for building the API
- **JSON** – Data format for requests/responses

---

## 📂 Project Structure

📁 project/ ├── modelo_diamantes.ipynb # Jupyter notebook for training and preprocessing ├── model.pkl # Serialized ML model ├── train.json # Training data ├── test.json # Test data ├── predictions.json # Prediction results ├── api/ │ ├── app.py # Main Flask app │ └── routes.py # API endpoints └── README.md # Project documentation


---

## 🔮 Potential Future Applications

- 💍 **E-commerce**: Use for dynamic diamond pricing on online marketplaces.
- 📊 **Business Intelligence**: Analyze trends in diamond pricing based on features.
- 🧠 **Educational**: Demonstrate ML pipelines and API building in classrooms.
- ⚙️ **Automation**: Retrain the model regularly with new data.
- 🔍 **Advanced Filters**: Expand filters to include clarity, carat, price range, etc.

---

## 📍 API Endpoints

- `GET /train` – Returns training dataset
- `GET /test` – Returns test dataset
- `GET /predictions` – Returns predictions from the model
- `GET /filter?color=G&cut=Ideal` – Returns diamonds filtered by color and cut

---

## 🔗 Demo

Try out the project interactively on [Gamma.app](https://gamma.app)

---

## 🛠️ Getting Started

```bash
# Clone the repo
git clone https://github.com/ShirleiO/API_Proyecto.git
cd API_Proyecto

# (Optional) Create a virtual environment
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate

# Install requirements
pip install -r requirements.txt

# Run the Flask app
python api/app.py
