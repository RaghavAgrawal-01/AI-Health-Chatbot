🩺 AI Health Chatbot :

- An AI-powered healthcare chatbot that predicts possible diseases based on user-reported symptoms using Machine Learning.  
- The system interacts with users, understands symptoms even with spelling mistakes, and provides disease predictions along with precautions and supportive messages.


🚀 Project Highlights :

- 🤖 Interactive Command Line Chatbot
- 🧠 Machine Learning (Random Forest Classifier)
- 🔍 Symptom detection with:
  - Exact matching
  - Synonym handling
  - Fuzzy matching (typos)
- 📊 Prediction confidence score
- 📖 Disease description
- 🛡️ Precaution suggestions
- 💬 Empathy-based health quotes


🛠️ Technologies Used :

- Python
- Pandas
- NumPy
- Scikit-learn
- Random Forest Algorithm
- CSV-based Medical Dataset


📁 Project Structure :

AI-Health-Chatbot/
│
├── Data/
│   ├── Training.csv
│   └── Testing.csv
│
├── MasterData/
│   ├── symptom_Description.csv
│   ├── symptom_severity.csv
│   └── symptom_precaution.csv
│
├── app.py
├── requirements.txt
└── README.md


⚙️ Installation Steps:

1. Clone the repository:

git clone https://github.com/RaghavAgrawal-01/AI-Health-Chatbot.git

2. Go to the project directory:

   cd AI-Health-Chatbot

3. Install required packages:

   pip install -r requirements.txt


▶️ How to Run the Project :

	python app.py


💬 Sample Output :

🤖 Welcome to HealthCare ChatBot

👉 What is your name? : Rahul

👉 Describe your symptoms: I have fever and stomach pain

✅ Detected symptoms: fever, stomach_pain

🩺 Based on your answers, you may have Dengue

🔎 Confidence: 86.75%

📖 About:

Dengue is a mosquito-borne viral infection causing high fever and body pain.

🛡️ Suggested precautions:
1. Drink plenty of fluids
2. Take adequate rest
3. Avoid mosquito exposure
4. Consult a doctor if symptoms worsen

⚠️ Disclaimer :
This chatbot is built for educational purposes only.
It is not a substitute for professional medical advice.
Always consult a certified doctor for medical concerns.


🔍 Model Workflow :
1. The user enters symptoms in natural language
2. Text preprocessing and symptom extraction are performed
3. Symptoms are converted into a binary feature vector
4. The Random Forest Classifier predicts the disease
5. A confidence score is calculated
6. Disease description and precautions are displayed


📊 Dataset Information : 
- The dataset is stored in CSV format
- Training and testing data are maintained in separate files
- Each row represents a disease
- Columns represent symptoms (1 = symptom present)
- Target column: `prognosis`

📁 Data Sources:
- `Data/Training.csv`
- `Data/Testing.csv`
- `MasterData/` (descriptions, severity, precautions)


🧠 Machine Learning Model :

- Algorithm Used: Random Forest Classifier
- Number of Trees: 300
- Train-Test Split: 67% training and 33% testing
- Label Encoding is used for the target variable
- The model provides probability-based confidence scores
