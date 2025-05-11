Botnet Detection in IoT Devices Using Machine Learning
This project aims to detect botnet attacks in IoT devices using machine learning algorithms. The increasing connectivity of IoT devices has made them vulnerable to various cyberattacks, especially botnets like Mirai and Gafgyt. This project utilizes the N-BaIoT dataset and applies supervised learning methods to classify malicious and benign traffic effectively.

📁 Dataset
N-BaIoT Dataset

Source: N-BaIoT Kaggle Dataset.

Devices: IoT devices including security cameras, baby monitors, and more.

Data: Network traffic (.csv) containing benign and attack (Mirai/Gafgyt) flows.

💡 Features
Data preprocessing & feature extraction

Label encoding of attack types

Machine learning classifiers: Random Forest, Decision Tree, Logistic Regression

Evaluation using Accuracy, Precision, Recall, F1-Score, Confusion Matrix

🧪 Models Used
Model	Description
Random Forest	Ensemble-based classifier with high accuracy
Decision Tree	Simple, interpretable model
Logistic Regression	Linear classifier for binary/multiclass output

📝 Requirements
Python 3.8+

pandas

numpy

scikit-learn

matplotlib

seaborn

Install dependencies:

bash
Copy
Edit
pip install -r requirements.txt
You can generate a requirements.txt using:

bash
Copy
Edit
pip freeze > requirements.txt
🧠 How It Works
Data Loading
Loads the benign_traffic.csv and attack traffic from each device subfolder.

Preprocessing

Removes null values

Combines benign and attack data

Encodes labels (e.g., Mirai, Gafgyt, Benign)

Training & Evaluation

Splits into train/test sets

Trains models and evaluates with metrics

Results Visualization

Confusion matrix

Accuracy comparison plot for all models

📊 Results
The Random Forest model outperformed others with:

Accuracy: ~99%

High F1-scores for all attack classes

📂 Project Structure
bash
Copy
Edit
├── botnet.ipynb                # Main notebook
├── data/                       # N-BaIoT dataset folders
│   ├── Device_1/
│   ├── Device_2/
│   └── ...
└── README.md                   # Project documentation
🚀 Usage
Clone this repository:

bash
Copy
Edit
git clone https://github.com/https://github.com/mayanksaini9/botnet-detection-iot.git
cd botnet-detection-iot
Download the N-BaIoT dataset and place it in the data/ folder.

Open and run the notebook:

bash
Copy
Edit
jupyter notebook botnet.ipynb
📌 Notes
One device (Samsung_SNH_1011_N_Webcam) lacks Mirai data.

The models can be further improved using deep learning or feature engineering.

📚 References
N-BaIoT: Network-Based Detection of IoT Botnet Attacks

dataset link : https://archive.ics.uci.edu/dataset/442/detection+of+iot+botnet+attacks+n+baiot
