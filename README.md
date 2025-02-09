# IoT-Based Maternal Health Monitoring System

## Problem Statement
Pregnant women, especially those at high risk, require continuous monitoring of their vital health parameters to ensure maternal and fetal well-being. However, traditional healthcare systems face challenges such as:
- Limited accessibility to real-time health data
- Delayed diagnosis of complications
- Difficulty in tracking symptoms over time
- Lack of structured documentation of daily experiences, symptoms, and concerns

There is a need for an **IoT-based vitals recording and tracking system** that integrates **wearable technology, cloud storage, AI-driven analysis, and telehealth services** to enable real-time monitoring, early risk detection, and seamless doctor-patient interaction. This solution aims to:
- Enhance maternal healthcare through **timely interventions**
- Provide **personalized insights**
- Offer **community support**
- Reduce pregnancy-related complications
- Improve maternal and fetal outcomes

## Features and Functionality
- **IoT-based vitals tracking** with real-time visualization on a **dashboard**
- **Self-tests** using **Gemini API**
- **NLP-based journal** for symptom tracking, which calculates complication risks and sends reports to doctors
- **AI-powered complication detection** to analyze symptoms and determine risk percentages
- **Digital scrapbook** (Journal and Memory Store) for patient health records
- **Doctor-Patient Connect** for seamless communication
- **Appointment reminders and notifications** for timely checkups
- **General health assistant bot** for common queries and guidance
- **Separate Dashboards** for **Doctors and Patients**
- **Doctor's Inbox** to categorize patient data based on risk levels, with an **important section** for high-risk cases

## Tech Stack
- **Frontend:** [Next.js](https://nextjs.org/)
- **Backend:** [Flask (Python)](https://flask.palletsprojects.com/)
- **Database:** [MongoDB](https://www.mongodb.com/)
- **Data Visualization:** [Chart.js](https://www.chartjs.org/)

## How to Set Up the Project
### Prerequisites
Ensure you have the following installed:
- Node.js & npm
- Python & Flask
- MongoDB

### Installation Steps
1. **Clone the Repository**
   ```sh
   git clone https://github.com/your-repo/iot-maternal-health.git
   cd iot-maternal-health
   ```
2. **Set Up the Backend**
   ```sh
   cd backend
   pip install -r requirements.txt
   python app.py
   ```
3. **Set Up the Frontend**
   ```sh
   cd frontend
   npm install
   npm run dev
   ```
4. **Set Up MongoDB**
   - Start MongoDB server locally or use **MongoDB Atlas**

## Usage
- Patients can **log in**, track their **vitals**, update their **journal**, and book **appointments**
- Doctors can **monitor high-risk cases**, check **complication reports**, and manage **appointments**

## Contributing
We welcome contributions! Feel free to **fork** the repository and create a **pull request**.

## License
This project is licensed under the **MIT License**.

## Contact
For any inquiries, reach out to:
- **Email:** sakshijaiswal1683@gmail.com

```mermaid
graph TD;
    IoT-Devices -->|Vitals Data| Backend(Flask API)
    Backend -->|Stores Data| Database(MongoDB)
    Backend -->|Sends Data| Frontend(Next.js)
    Frontend -->|Doctor-Patient Interaction| Dashboard
    Dashboard -->|Alerts & Reports| Doctor
    Dashboard -->|Health Insights| Patient


