# Renewable Energy Generation Prediction

This project implements a machine learning model to predict renewable energy generation using XGBoost. The model is deployed as a web application using Flask, allowing users to make predictions through an interactive interface.

## Project Structure

```
Project Code/
├── ML_Model/
│   ├── XGB_renewable_energy_prediction.ipynb  # Main Jupyter notebook for model development
│   ├── Turbine_Data.csv                       # Dataset used for training
│   ├── model1.json                           # First trained model
│   ├── model2.json                           # Second trained model
│   ├── model2.pkl                            # Pickled model file
│   └── app/                                  # Flask web application
│       ├── app.py                            # Main Flask application
│       ├── model.py                          # Model loading and prediction functions
│       ├── static/                           # Static files (CSS, images)
│       └── templates/                        # HTML templates
```

## Features

- XGBoost-based prediction model for renewable energy generation
- Web interface for easy prediction
- Interactive date range selection
- Visual representation of predictions using matplotlib
- Responsive design with CSS styling

## Technologies Used

- Python
- XGBoost
- Flask
- Pandas
- NumPy
- Matplotlib
- Seaborn

## Setup and Installation

1. Clone the repository:

```bash
git clone <your-repository-url>
```

2. Install the required dependencies:

```bash
pip install flask pandas numpy xgboost matplotlib seaborn
```

3. Navigate to the app directory:

```bash
cd Project\ Code/ML_Model/app
```

4. Run the Flask application:

```bash
python app.py
```

5. Open your web browser and visit `http://localhost:5000`

## Usage

1. Enter the desired date range for prediction in the format "yyyy-mm-dd"
2. Click the "predict" button
3. View the generated prediction chart

## Model Details

The model uses the following features for prediction:

- Hour
- Minute
- Day
- Month
- Year
- Day of week
- Day of year

## Note

The model's accuracy may decrease for predictions far into the future from the last recorded date (01/04/2020) in the dataset.

## Contributing

[Add contribution guidelines if applicable]
