# Diabetic-Retinopathy-Project
A Django-based web application that uses a deep learning model to detect Diabetic Retinopathy and related eye conditions from retinal images.


Title & Description
# Deep Diabetic — Identification System of Diabetic Eye Disease using Deep Neural Networks

A Django-based web application that uses a deep learning (CNN) model to detect Diabetic Retinopathy and Macular Edema from retinal (fundus) images.

## Features
- User & Admin web portals (registration, login, upload)
- Upload a retinal image and get an automated prediction
- Trained Keras/TensorFlow CNN model (`model/retinopathy_model.h5`)
- Image preprocessing pipeline using OpenCV

- ## Tech Stack
- **Backend:** Django (Python)
- **Deep Learning:** TensorFlow / Keras
- **Image Processing:** OpenCV, imutils
- **Database:** SQLite (default, swappable)

- ## Project Structure
```
DiabeticRetinopathy/
├── AdminApp/          # Admin-side Django app
├── UserApp/           # User-side Django app
├── model/             # Trained deep learning model
├── Static/            # CSS, JS, images
├── Templates/          # HTML templates
├── testSamples/         # Sample fundus images for testing
└── manage.py
```

## Setup & Installation

1. Clone the repository
```bash
   git clone <your-repo-url>
   cd DiabeticRetinopathy
```

2. Create a virtual environment and install dependencies
```bash
   python -m venv venv
   source venv/bin/activate   # Windows: venv\Scripts\activate
   pip install -r requirements.txt
```

3. Set your Django secret key (recommended)
```bash
   export DJANGO_SECRET_KEY="your-own-random-secret-key"
```

4. Run migrations and start the server
```bash
   python manage.py migrate
   python manage.py runserver
```

5. Open `http://127.0.0.1:8000/` in your browser.

## Setup & Installation

1. Clone the repository
```bash
   git clone <your-repo-url>
   cd DiabeticRetinopathy
```

2. Create a virtual environment and install dependencies
```bash
   python -m venv venv
   source venv/bin/activate   # Windows: venv\Scripts\activate
   pip install -r requirements.txt
```

3. Set your Django secret key (recommended)
```bash
   export DJANGO_SECRET_KEY="your-own-random-secret-key"
```

4. Run migrations and start the server
```bash
   python manage.py migrate
   python manage.py runserver
```

5. Open `http://127.0.0.1:8000/` in your browser.

 ## Dataset
The training dataset (fundus images, categorized into Diabetic Retinopathy / Macular Edema / No Disease) is not included in this repository due to its size. Please source a diabetic retinopathy dataset (e.g., APTOS/Kaggle) and organize it into the same folder structure as `Dataset/` before retraining.

## Disclaimer
This project is for academic/research purposes only and is **not** a certified medical diagnostic tool.
   
