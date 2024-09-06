**House Price Prediction with Flask and Vercel Deployment**
This project demonstrates a simple machine learning model for predicting house prices. The model is trained using a basic linear regression algorithm, and the deployment is managed through Flask with an interactive web interface. GitHub Actions is used to automatically deploy the project on Vercel whenever changes are pushed to the main branch.

**Features**
Linear Regression Model: Predicts house prices based on a set of input features.
Flask Web Application: Users can enter the required features via a simple web form, and the app will return the predicted house price.
Automated Deployment: GitHub Actions is configured to deploy the project to Vercel upon each push to the main branch.

**Tech Stack**
Python 3.x
Flask for web framework
Scikit-learn for machine learning
HTML/Jinja2 for frontend forms
GitHub Actions for CI/CD
Vercel for hosting and deployment

.**Project Structure:**
├── app.py                # Main Flask application
├── model_training.py      # Script to train the model
├── house_model.pkl        # Trained model file
├── templates
│   └── form.html          # HTML form for user input
├── requirements.txt       # Project dependencies
├── .github
│   └── workflows
│       └── deploy.yml     # GitHub Actions configuration for deployment
└── vercel.json            # Vercel deployment configuration

**Prerequisites**
Before running the project locally, ensure you have the following installed:
Python 3.x
Node.js and npm (for Vercel deployment)
A Vercel account (Sign up here)
Installation

**Clone the repository:**
git clone https://github.com/your-username/your-repo-name.git
cd your-repo-name
Install the required Python dependencies:
Copy code
pip install -r requirements.txt

**Train the model:**
python model_training.py

**Run the Flask app:**
python app.py
Access the web app at http://127.0.0.1:5000/.
Deployment
Using GitHub Actions and Vercel
This project is set up to automatically deploy to Vercel via GitHub Actions. Follow these steps to configure it:

**Generate a Vercel Token:**

Visit Vercel Tokens and create a new token.
Set Up GitHub Secrets:

In your GitHub repository, navigate to Settings > Secrets and variables > Actions.
Add a new secret with the name VERCEL_TOKEN and paste the Vercel token you generated.
Push Your Code:

Every time you push changes to the main branch, GitHub Actions will automatically deploy your project to Vercel.
