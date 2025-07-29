# Animal Disease Severity Prediction using Machine Learning

This project is a web-based machine learning application that predicts whether an animal's disease is dangerous (severe) or not dangerous (normal) based on the animal name and five reported symptoms.

📁 Project Structure
The project is organized into a structured directory for clarity and modularity. The app.py file serves as the Flask backend that handles form submissions and predictions. The train_model.py script is used to train the machine learning model from dataset.csv and save it as disease_model.pkl. The templates/ folder contains the index.html file, which provides a user interface for inputting animal names and symptoms. The optional static/ folder holds styling files like style.css. All project documentation is included in the README.md file, giving an overview of usage and structure. This setup allows for easy development, training, and deployment of the animal disease prediction system.

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
Click Predict.
You’ll see:
No, it is not dangerous. (Normal)
Yes, it is dangerous. (Severe)

*Model Used*
Model: Random Forest Classifier
Input Features: AnimalName, symptoms1 to symptoms5
Target: Dangerous (Yes / No)
