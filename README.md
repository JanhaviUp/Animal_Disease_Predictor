# Animal Disease Severity Prediction using Machine Learning

This project is a web-based machine learning application that predicts whether an animal's disease is dangerous (severe) or not dangerous (normal) based on the animal name and five reported symptoms.

📁 Project Structure
animal_disease_prediction/
│
├── app.py                # Flask app backend
├── disease_model.pkl     # Trained ML model
├── templates/
│   └── index.html        # Frontend form for prediction
├── static/
│   └── style.css         # (Optional) Add styles here
├── dataset.csv           # Input dataset used to train the model
├── train_model.py        # Python script to train and save the model
└── README.md             # Project documentation

⚙️ Requirements
Install required libraries:
pip install flask pandas scikit-learn

*How to Run the Project*
1. Train the model (if not already trained)
python train_model.py
This will generate disease_model.pkl.

*2. Run the Flask app*
python app.py
You should see output like:
Running on http://127.0.0.1:5000/ (Press CTRL+C to quit)

*3. Open the App in Browser*
Open your browser and go to: http://127.0.0.1:5000

How to Use
Enter the animal name (e.g., Dog, Cat, Cow).
Fill in all five symptoms (case-insensitive).
Click Submit.
You’ll see:
✅ No, it is not dangerous. (Normal)
⚠️ Yes, it is dangerous. (Severe)

*Model Used*
Model: Random Forest Classifier
Input Features: AnimalName, symptoms1 to symptoms5
Target: Dangerous (Yes / No)
