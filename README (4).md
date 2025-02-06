# 🛡️ Real-Time Malicious URL Detection and Protection System using Lexical Analysis



**Real-Time Malicious URL Detection and Protection System** is an innovative cybersecurity solution that leverages machine learning and advanced lexical analysis to proactively detect and thwart malicious URLs. This repository contains a multi-faceted system comprising a Chrome extension for instantaneous protection, a robust machine learning model for URL classification, and a web interface for manual URL verification.

Lexical analysis here refers to the process of deconstructing a URL into its elemental components (such as domain, subdomain, path, and parameters) to extract discerning features. These features—like URL length, character frequencies, and special symbol usage—enable the system to distinguish benign URLs from those that could potentially compromise security.

## System Requirements

![Python](https://img.shields.io/badge/Python-3.7%2B-blue?style=flat&logo=python) ![Flask](https://img.shields.io/badge/Flask-API%20Development-orange?style=flat&logo=flask) ![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-red?style=flat&logo=jupyter) ![Chrome](https://img.shields.io/badge/Chrome-Browser-green?style=flat&logo=google-chrome)

- **Hardware:**  
  - Minimum 4 GB RAM  
  - Intel i5 (7th Gen) processor or higher  
  - At least 256 GB of storage

- **Software:**  
  - Python 3.7 or lower  
  - Flask for API development  
  - Web browsers: Google Chrome, Firefox  
  - Jupyter Notebook for development and testing

## 🚀 Features

- **Real-Time Detection:**  
  The system intercepts URL requests and performs rapid, on-the-fly analysis to alert users about potential threats.

- **Machine Learning Integration:**  
  Utilizes a Random Forest classifier, which aggregates the decisions of multiple decision trees, to achieve high accuracy in identifying malicious URLs (95% accuracy, with a balanced precision and recall).

- **Chrome Extension:**  
  A custom-built extension seamlessly integrates with Google Chrome to provide real-time protection by warning users before they access dubious websites.

- **Web Interface for Manual Checking:**  
  Offers a user-friendly webpage where users can manually input URLs and receive a comprehensive safety analysis, including a confidence score.

- **Comprehensive Lexical Feature Extraction:**  
  The system meticulously analyzes URL components—such as lexical structure, special character frequency, and domain attributes—to ascertain the maliciousness of a URL.

## 🏗️ System Architecture

The architecture of the system is delineated into three principal components:

1. **Chrome Extension:**  
   Acts as the frontline defense by capturing URL requests and communicating with the backend for immediate classification.

2. **Machine Learning Model:**  
   Developed in Python, this component employs supervised learning techniques (Random Forest, SVM, Naive Bayes) to classify URLs based on a pre-processed feature set.

3. **Web Interface:**  
   Built using HTML, CSS, JavaScript, and Flask, it allows users to manually verify URLs and provides educational safety tips.



## ⚙️ Installation

1. **Clone the Repository:**

   ```bash
   git clone https://github.com/yourusername/RealTimeMaliciousURLDetection.git
   cd RealTimeMaliciousURLDetection
   ```


2. **Create a Virtual Environment and Install Dependencies:**

   ```bash
   python3 -m venv venv
   cd ChromeExtensionPart
   source venv/bin/activate  # On Windows, use: venv\Scripts\activate
   pip install -r requirements.txt
   ```

3. **Run the Backend Server:**

   ```bash
   python web.py
   ```

4. **Load the Chrome Extension:**
   - Open Chrome and navigate to `chrome://extensions/`.
   - Enable "Developer Mode."
   - Click on "Load unpacked" and select the `extension` folder.

## Usage

- **Real-Time Protection:**  
  Once the extension is active, it automatically intercepts and analyzes URLs in real time, providing immediate alerts if a URL is determined to be malicious.

- **Manual URL Checking:**  
  Navigate to the web interface (`http://localhost:5000/` by default) to input any URL for a detailed safety analysis, which includes a classification label (safe/malicious) and a confidence score.

## Testing and Validation

The system undergoes rigorous functional, performance, and security testing to ensure reliability:
- **Functional Testing:** Validates correct URL classification and error handling.
- **Performance Testing:** Ensures rapid URL analysis (typically under 1–2 seconds) even under high loads.
- **Security Testing:** Verifies the robustness of the system against adversarial attacks and vulnerabilities.

## Conclusion

This project epitomizes a harmonious blend of machine learning and lexical analysis to fortify online security in real time. It not only detects malicious URLs with high precision but also educates users on safe browsing practices, thereby engendering a safer digital ecosystem.

---

*Glossary:*  
- **Lexical Analysis:** The process of breaking down text (here, URLs) into meaningful elements for further processing.  
- **Random Forest:** An ensemble machine learning method that constructs multiple decision trees during training and outputs the mode of the classes for classification.

Feel free to explore, contribute, and adapt this project for enhanced cybersecurity applications!


---

