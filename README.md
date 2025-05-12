# CatchThePhish

**CatchThePhish** is a machine learning-based web application that detects phishing websites. Users can register or log in to input URLs, which are then analyzed using a trained model to classify them as either *phishing* or *legitimate*. Detected phishing URLs are stored in a local database and can be downloaded.

---

## 🚀 Features

- **Login/Register System**: Secure user authentication.
- **URL Prediction**: Input a URL to check if it’s phishing or legitimate.
- **Feature Extraction**: Uses 35+ URL-based features for accurate prediction.
- **Model Used**: Random Forest Classifier.
- **Phishing URL Storage**: Saves flagged phishing URLs locally.
- **Blacklist Check** *(optional)*: Integrates with Google Safe Browsing API.
- **Download List**: Allows download of flagged phishing URLs as a `.txt` file.

---

## 📁 Project Structure

- `app.py`: Main Flask application with URL prediction logic and model integration.
- `auth.py`: Handles user authentication (login, registration, password recovery).
- `phishing_detection_model.pkl`: Pre-trained ML model.
- `dataset_phishing.csv`: Dataset used for training/testing the model.
- `templates/`: HTML templates (login, register, home, results, etc.).
- `static/`: CSS and JS assets for UI styling (optional).

---

## 🛠️ Installation

1. **Clone the Repository**
   ```bash
   git clone https://github.com/yourusername/phishing-website-detector.git
2. **Navigate to the Project Directory**
   ```bash
   cd CatchThePhish
3. **Install Required Dependencies**
   ```bash
   pip install -r requirements.txt
4. **Run the Application**
   ```bash
   python app.py

## 📌 Usage

- **Register/Login**: Create an account or log in with your credentials.
- **Check URLs**: Enter a URL in the input form to check if it's phishing.
- **Download Detected URLs**: Navigate to `/download_phishing_urls` (after login) to download the list of flagged phishing URLs.

