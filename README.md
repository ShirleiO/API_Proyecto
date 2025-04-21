# 💎 Diamond Price Prediction API

This project provides an API interface for predicting diamond prices using machine learning. It was developed using a structured dataset of diamond features, a trained regression model, and integrated with interactive tools for querying and visualization.

---

## 🚀 Features

- **Train/Test Split**: Dataset split into training and test subsets for model evaluation.
- **Model Deployment**: A regression model was trained and saved using `pickle`.
- **JSON Integration**: Unified data frames (train, test, predictions) stored in JSON format.
- **API Routes**:
  - Serve different datasets (Train, Test, Predictions)
  - Filter by **Color** and **Cut**

---

## 📦 Tech Stack

- **Python** – Data manipulation and backend development
- **Pandas** – Data processing
- **Scikit-learn** – Model training
- **Pickle** – Model serialization
- **JSON** – Standard data format for API and storage
- **API Framework** – (Flask)

---

## 📍 Example Endpoints

- `GET /train` – Returns training dataset
- `GET /test` – Returns test dataset
- `GET /predictions` – Returns predicted diamond prices
- `GET /filter?color=G&cut=Ideal` – Filter diamonds by attributes

---

## 🔮 Potential Future Applications

- **E-commerce**: Price calculators and smart filters for diamond shopping.
- **Market Analytics**: Tools for identifying pricing trends in the gem industry.
- **Education**: Use case for teaching regression and API deployment.
- **Model Evolution**: Incorporate new training data and dynamic updates.
- **Extended Filtering**: Add parameters like **Clarity**, **Carat**, or **Certification**.

---

## 🔗 Related Tools

- [Gamma.app](https://gamma.app) – Used for query demonstrations and data visualization.

---

## 🛠️ Getting Started (Example)

```bash
# Clone the repo
git clone https://github.com/your-username/diamond-price-api.git
cd diamond-price-api

# Install dependencies (example if using Flask)
pip install -r requirements.txt

# Run the app
python app.py
