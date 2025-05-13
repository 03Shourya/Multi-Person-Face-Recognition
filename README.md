MIT license
📸 Multi Person Face Recognition

Doc Fusion is a Flask-based web application that uses Dlib and OpenCV to perform face recognition on uploaded video files or live IP camera streams. It also allows email alerts with detection summaries using Gmail APIs.
Preview


🚀 Features

🎥 Upload and analyze stored videos
📡 Real-time inference from IP camera streams
🧠 Face recognition using multi-frame processing with Dlib
📄 Export detection summary as CSV
📧 Email alerts with summary reports
🔐 Secure session handling with Flask
🔍 Input validation and error handling
🛠️ Setup Instructions

Step 1: Create a Virtual Environment
python3 -m venv myenv
Step 2: Activate the Environment
source myenv/bin/activate
Step 3: Upgrade pip
pip3 install --upgrade pip
Step 4: Install System Libraries for Video Support
sudo apt update -y && sudo apt install ffmpeg libsm6 libxext6 -y
Step 5: Install Dependencies for Dlib & Face Recognition
sudo apt install cmake libboost-all-dev build-essential -y
Step 6: Install Python Dependencies
pip3 install -r requirements.txt
Step 7: Install Gmail API Libraries
pip3 install --upgrade google-api-python-client google-auth-httplib2 google-auth-oauthlib
🧪 Running the App

python -m flask --app src/app.py run --host=0.0.0.0
📸 Supported Video Formats

MP4
MOV
AVI
WMV
Note: Max video size = 200MB
📬 Email Alert Configuration

Ensure you've set up Gmail OAuth credentials and enabled Gmail API access via Google Cloud Console. Configure sender details in parameters.py.
🤝 Contributing

Feel free to fork, raise issues or submit pull requests!
📄 License

This project is licensed under the MIT License.
