This is an end-to-end machine learning project to predict house prices in Bangalore, India. It includes data cleaning, model training, and a web application to make real-time predictions.

## 🔧 Features
- Data Preprocessing: Handles missing values and outliers.
- Model Training: Uses a regression model (e.g., Linear Regression, Random Forest).
- Web Application: A user-friendly interface built with Flask for making predictions.
- Minimal Dependencies: The project is easy to set up and run.
- Deployment Ready: The structure is set up for easy deployment on platforms like Heroku.

## 📁 Project Structure

<pre>
BLR-House-Price-Prediction/
├── BLR_House_Price_Prediction.ipynb
├── app.py
├── artifacts/
│   ├── bangalore_home_prices_model.pickle
│   └── columns.json
├── data/
│   └── Bengaluru_House_Data.csv
├── templates/
│   └── app.html
├── requirements.txt
└── static/
</pre>

## 🚀 How to Use

1. Set up the Environment
Make sure you have Python installed. We recommend using a virtual environment.

First, clone the repository:

```bash
git clone https://github.com/Saiyanav/BLR-House-Price-Prediction.git
cd BLR-House-Price-Prediction
```

Then, create and activate the virtual environment and install the required dependencies:

```bash
# On macOS and Linux
python3 -m venv venv
source venv/bin/activate
pip install -r requirements.txt
```

```bash
# On Windows
python -m venv venv
.\venv\Scripts\activate
pip install -r requirements.txt
```

2. Train the Model
The model is trained in the BLR_House_Price_Prediction.ipynb Jupyter Notebook. To re-train or inspect the process, open the notebook and run all the cells. This will generate the model artifacts (.pickle file and columns.json) in the artifacts/ folder.

```bash
jupyter notebook
```

3. Run the Web Application
After the model is trained and the dependencies are installed, you can start the Flask web server:

```bash
python3 app.py
```

Open your web browser and go to http://127.0.0.1:5000/ to use the prediction tool.

## 🏠 Example Output
!(https://i.imgur.com/your-screenshot-link-here.png)

(Note: You can replace the image link above with a screenshot of your own web application's output.)

## 📝 Notes
The model is trained on the Bengaluru_House_Data.csv dataset, which is a key component of the project.

The prediction output is based on the features you provide: location, square feet, BHK (bedrooms), and bathrooms.

The artifacts/ directory stores the trained model and a file for column information, which the web app uses for prediction.