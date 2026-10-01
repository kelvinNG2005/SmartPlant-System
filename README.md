# **🌿 SmartPlant System**

SmartPlant is an AI-powered mobile application designed to help users identify plants, visualize geographical growing patterns, protect plantations using IoT monitoring, and ensure user data privacy through secure backend architecture. The system also includes automated AI retraining to support continuous learning and improvement.
   
##  **🚀 Key Features**

- **AI-Powered Mobile Plant Identification**
- **Visualization & Mapping Tools**
- **IoT-Enabled Plant Protection Alerts**
- **Cybersecurity & Data Privacy Controls**
- **Automated AI Model Retraining Module**

## **👤 My Contribution**
AI Model Management & Deployment

My primary contribution focused on the AI model management lifecycle and AI backend deployment.

Designed and implemented an automated AI retraining workflow based on newly verified plant observations and administrator-configured thresholds.
Integrated verified user-submitted plant images into the AI training data lifecycle.
Implemented the workflow for triggering model retraining when the configured data threshold is reached.
Developed the model evaluation and replacement workflow, using validation performance to determine whether a newly trained model should become the active model.
Deployed and configured the Python AI classification backend to provide plant identification services to the main application.
Integrated the AI backend with the main system to support plant identification and model management functionality.



##  **🛠️ Local Development Setup**

##  **1\. Clone the Repository**

```console
git clone <https://github.com/thelazycat-0728/COS30049>

cd COS30049
```

##  **2\. Install Dependencies**

**Frontend**

```console
cd frontend

npm install

```

**Backend**
``` console
cd ..

cd backend

npm install

```

**AI Backend**

``` console
cd ..

cd ai-backend

npm install

pip install -r requirements.txt

```

##  **3\. Configure Environment Variables**

Locate the following .env files and update the IP address to match **your local machine**:

- frontend/.env
- backend/.env

**Important:** Include the http:// prefix and ensure the backend port matches across configurations.

If **port 8080** is already in use, change it in:

| **File Location** | **Variable Name** |
| --- | --- |
| frontend/.env | EXPO_PUBLIC_API_BASE |
| backend/.env | PORT |
| backend/.env | MAIN_BACKEND_URL |

##  **4\. Run the Project**

Run the following services **simultaneously**:

**Frontend**

``` console
cd frontend

npm run start

```

**Backend**

```console
cd backend

npm start

```

**AI Backend**
``` console
cd ai-backend

npm start

```

**❗ Troubleshooting**

| **Issue** | **Fix** |
| --- | --- |
| **Network error during login** | Check frontend/.env and ensure correct IP + port format (e.g., <http://192.168.0.10:8080>) |
| **Port already in use** | Update ports in .env files as described above |
| Backend not responding | Ensure all three components are running |

##  **🔧 IoT Setup**

Refer to the **Readme file inside the /IoT folder** for hardware and firmware configuration instructions.

##  **☁️ Cloud Deployment**

##  **Steps:**

- Clone the cloud branch
- Request the project owner (**Jonathan**) to activate the cloud server.

AWS Educate learner accounts require manual server activation when starting the lab environment.

- Run the frontend locally as usual.
- **Skip the backend step** - backend runs remotely in AWS.
- Contact the AI engineer (**Kelvin**) to deploy the AI backend server.  
    Once deployed, AI features (plant detection, retraining, etc.) will be functional.

##  **📄 License**

This project is for academic and demonstration purposes. License terms may be updated based on deployment requirements.

##  **📞 Support / Contacts**

For assistance during setup:

| **Area** | **Contact** |
| --- | --- |
| Cloud backend server | **Jonathan** |
| AI model & AI backend | **Kelvin** |
| General project issues | Any contributing member |
