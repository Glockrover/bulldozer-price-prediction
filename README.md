# 🚜 Bulldozer Sale Price Prediction

Predict the sale price of bulldozers using historical sales data and machine learning models. 🤖📊

## 🔍 Problem

Predict the future sale price of a bulldozer based on its characteristics and past sales. 🎯💰

## 📂 Data

Train.csv: Sales data up to 2011 🗓️

Valid.csv: Validation data (Jan–Apr 2012) 🧪

Test.csv: Test data (May–Nov 2012) 🏁

All feature definitions are available in the Kaggle competition’s data dictionary 📝

## ⚙️ Features

Examples of key features:

* YearMade – Year the bulldozer was manufactured 🏗️

* MachineHoursCurrentMeter – Current meter reading ⏱️

* ModelID – Model identifier 🆔

## 🛠️ Modelling

We used a RandomForestRegressor to predict sale prices. Key steps:

* 🕒 Datetime Features: Parse and extract features from saledate.

* 🔢 Categorical Encoding: Convert string categories to numerical codes.

* 🧩 Missing Values: Fill missing numeric values with median and add missingness indicators.

* 📊 Data Split: Train on 2011 and earlier, validate on 2012.

* ⚙️ Hyperparameter Tuning: RandomizedSearchCV on a subset of the training set.

* 🏋️‍♂️ Final Model: Train on full dataset using best parameters.

## 🧮 Prediction

Apply preprocessing to test data.

Predict sale prices with the trained model.

Output predictions for Kaggle evaluation 🎯📦

## 🚀 Getting Started
# Clone the repo
git clone https://github.com/yourusername/bulldozer-price-prediction.git
cd bulldozer-price-prediction

# Create virtual environment
python -m venv venv
source venv/bin/activate  # Linux/Mac
venv\Scripts\activate     # Windows

# Install dependencies
pip install -r requirements.txt

# Run the notebook
jupyter notebook Bulldozer_Price_Prediction.ipynb

## 💡 Key Takeaways

* Feature engineering (especially date features) boosts model performance 🗓️✨

* Handling missing values and categorical data is crucial 🧩✅

* Random Forests are robust for tabular regression 🌳💪
