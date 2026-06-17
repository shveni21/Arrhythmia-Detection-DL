# AI-Powered Cardiac Arrhythmia Detection System

CardioAI is a full-stack web application that uses a hybrid **CNN–GRU deep learning model** to automatically detect and classify cardiac arrhythmias from ECG signals. The platform connects **patients**, **doctors**, and **admins** in one system — patients upload ECG data for instant AI diagnosis, doctors review results and issue prescriptions, and admins manage users and system health.

The model classifies ECG signals into 5 classes (Normal, Supraventricular, Ventricular, Fusion, Unknown) and is trained on the MIT-BIH Arrhythmia Database, achieving **97.52% accuracy** by combining 1D-CNN spatial feature extraction with GRU-based temporal sequence modeling.

---

## 🏗️ Tech Stack

| Layer | Technology |
|---|---|
| Backend | Python, Flask |
| Machine Learning | TensorFlow / Keras, scikit-learn |
| Data Processing | Pandas, NumPy |
| Visualization | Matplotlib |
| Database | SQLite |
| PDF Reports | ReportLab |
| Auth | bcrypt |
| Frontend | Jinja2, Tailwind CSS, Bootstrap Icons |
| Email | SMTP (via `email_helper.py`) |

---

## 🚀 Usage

1. Sign up as a **Patient** or **Doctor** (or log in as **Admin** with default credentials).
2. As a patient, go to **ECG Detection** and upload a CSV file with 187 numeric ECG features (a sample file is downloadable from the app).
3. View the AI's classification, confidence score, and ECG signal plot instantly.
4. Download a PDF report or share the result with your doctor by email.
5. Doctors can review patient results and issue digital prescriptions.
6. Admins can manage users, monitor system stats, and export/back up data.


---

## 🔮 Future Improvements

- Extend training to additional ECG datasets (e.g., PTB-XL) for better real-world generalization
- Build a lightweight version of the model for real-time inference on wearable devices
- Integrate Explainable AI (XAI) techniques (e.g., SHAP, Grad-CAM) for interpretable predictions
- Add multi-lead ECG support and continuous monitoring streams
