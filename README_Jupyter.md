# 🚨 Intruder Detection System (Jupyter Notebook Version)

This project is an AI-based Intruder Detection System implemented in a **Jupyter Notebook** using computer vision techniques. It uses OpenCV and NumPy for video processing and motion detection, and sends real-time alerts via SMS using the Twilio API.

## 🧠 Features

- 📹 Video Feed Processing using OpenCV
- 🕵️ Motion Detection with Frame Differencing
- 📅 Timestamp Logging using `date` and `datetime`
- 📲 Real-Time SMS Alerts with Twilio API
- 📊 Jupyter Notebook Interface for Visualization and Prototyping

## 🔧 Technologies Used

- **Python**
- **OpenCV (`cv2`)** - For accessing webcam/video feed and image processing
- **NumPy** - For array manipulation and frame differencing
- **datetime & date** - For timestamping intruder events
- **Twilio** - To send SMS alerts when an intrusion is detected
- **Jupyter Notebook** - Interactive environment for development and testing

## 📁 Files Structure

```
intruder-detection-jupyter/
│
├── Intruder_Detection_System.ipynb   # Main Jupyter Notebook
├── requirements.txt                  # List of required packages
├── README.md                         # Project documentation
└── intrusion_logs.txt                # Optional log file of intrusion timestamps
```

## 📦 Installation

### Prerequisites

- Python 3.8+
- Jupyter Notebook or JupyterLab installed
- A webcam or video file source

### Setup Instructions

1. Clone the repository or download the notebook.
2. Install the required packages:

```bash
pip install numpy opencv-python twilio
```

3. Open the notebook:

```bash
jupyter notebook Intruder_Detection_System.ipynb
```

4. Configure your Twilio credentials in a code cell:

```python
TWILIO_ACCOUNT_SID = 'your_account_sid'
TWILIO_AUTH_TOKEN = 'your_auth_token'
FROM_PHONE = '+1234567890'         # Twilio phone number
TO_PHONE = '+0987654321'           # Your phone number
```

## 🚀 How It Works

- The notebook captures frames from your webcam or video file.
- Uses NumPy and OpenCV to detect motion through frame differencing.
- If motion is detected beyond a threshold, it sends an SMS alert via Twilio.
- Logs the event with the current date and time.

## 📸 Sample Output

> _Include screenshots or outputs from the notebook showing motion detection and alerts._

## 📜 License

MIT License

## 👨‍💻 Author

- [Shabbeer Basha](https://github.com/shabbeer08)

---

For educational and prototype purposes. Contributions are welcome!
