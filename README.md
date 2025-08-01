

# 🚗 Vehicle Insurance Prediction using MongoDB & Random Forest

This project demonstrates how to load data from a CSV file, store it in MongoDB Atlas, and train a Random Forest model using `scikit-learn` inside a Jupyter Notebook.

---

## 📁 Folder Structure

project-root/
├── vehicle.ipynb # Main notebook for data ingestion and model training
├── data.csv # Input dataset
├── .env # MongoDB credentials (NOT tracked by Git)
├── requirements.txt # List of dependencies
├── README.md # Project documentation

yaml
Copy
Edit

---

## ✅ Prerequisites

- Python 3.10+
- MongoDB Atlas account (free tier)
- Git
- Virtual environment (`venv`)
- Jupyter Notebook installed

---

## ⚙️ Setup Instructions

### 1. Clone the Repository
```bash
git clone https://github.com/your-username/vehicle-mlops-project.git
cd vehicle-mlops-project
2. Create and Activate a Virtual Environment
bash
Copy
Edit
python -m venv vehicle
source vehicle/bin/activate    # On Windows: vehicle\Scripts\activate
3. Install Required Dependencies
bash
Copy
Edit
pip install -r requirements.txt
4. Configure MongoDB Atlas Connection
Create a .env file in the root directory with the following content:

ini
Copy
Edit
MONGODB_URL=mongodb+srv://<username>:<password>@cluster0.mongodb.net/?retryWrites=true&w=majority&appName=Cluster0
Replace <username> and <password> with your MongoDB Atlas credentials.

⚠️ Make sure your .env file is added to .gitignore to avoid pushing it to GitHub.

🚀 How to Run the Notebook
Start Jupyter Notebook:

bash
Copy
Edit
jupyter notebook
Open vehicle.ipynb

Run the notebook cells in order to:

Load data.csv

Convert data to dictionary format

Upload data to MongoDB

Train a Random Forest classifier using RandomizedSearchCV

Evaluate model performance

🧪 Output
Data stored in MongoDB:

Database: vehicle_mlops

Collection: vehicle-data

Final model results printed (e.g., best parameters, accuracy)

🔐 Security Notes
Do not commit your .env file to GitHub.

Your .gitignore should include:

bash
Copy
Edit
.env
__pycache__/
*.log
logs/
📫 Maintainer
Bhavya Champaneri
If you have questions or want to collaborate, feel free to reach out.
