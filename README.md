# 🛡️ PhishGuard AI – LLM Edition

### Think Before You Click.

A browser-based message safety assistant that helps users identify potential phishing warning signs through rule-based analysis and a locally running AI model.

🌐 **Live Demo:** https://adi-bugata.github.io/PhishGuard-AI-LLM/

---

## 📌 Problem Statement

Phishing messages often use urgency, threats, fake rewards, and requests for sensitive information to trick people into sharing personal or financial details.

Many users struggle to distinguish suspicious messages from legitimate communication.

PhishGuard AI aims to make people more aware of these warning signs and encourage safer online decisions.

## 💡 Our Solution

PhishGuard AI combines a rule-based warning checklist with an AI-powered explanation to help users understand why a message may be suspicious.

Users can paste a message into the application and receive:
- A checklist warning score.
- Identified warning signs.
- An AI-generated explanation.
- A consistent safety assessment.
- Practical recommendations for safer decisions.

## ✨ Key Features

- **Rule-Based Detection:** Identifies common warning signs such as urgency, requests for sensitive information, suspicious links, prize claims, and payment requests.
- **Warning Score:** Displays a heuristic warning score out of 10.
- **AI-Powered Explanation:** Uses Qwen2.5-0.5B-Instruct to explain identified warning signs.
- **Browser-Based AI:** Runs model inference in the user's browser without a hosted AI inference API.
- **Safety Recommendations:** Provides consistent recommendations using JavaScript.
- **Simple Interface:** Offers an easy-to-use interface for analysing pasted messages.

## ⚙️ Technologies Used

| Technology | Purpose |
|---|---|
| HTML | Application structure |
| CSS | User interface and styling |
| JavaScript | Application logic and rule-based analysis |
| Transformers.js | Running the AI model in the browser |
| Qwen2.5-0.5B-Instruct | AI-generated explanations |
| GitHub Pages | Application hosting |

## 🔍 How It Works

PhishGuard AI follows a simple analysis workflow:

1. **Input:** The user pastes a suspicious message.
2. **Rule-Based Analysis:** JavaScript checks for predefined warning patterns.
3. **Warning Score:** The application calculates a heuristic score based on detected patterns.
4. **AI Explanation:** The message and identified warning signs are passed to the Qwen model running in the browser.
5. **Safety Assessment:** JavaScript presents a consistent assessment and practical safety recommendations.
6. **Output:** The user receives an explanation of potential warning signs and safer next steps.

## 🏗️ Architecture

```text
          User
            |
            v
      Message Input
            |
            v
     Rule-Based Analysis
            |
            v
      Warning Score
            |
            v
     AI Explanation
            |
            v
       Qwen2.5 Model
      (Browser-Based)
            |
            v
   JavaScript Safety Advice
            |
            v
      Analysis Results
```

## 🧪 Example Analysis

**Sample message:**

"Your bank account will be blocked today. Verify your account immediately by sharing your OTP. Click https://example.com to continue."

**Detected warning signs:**
- Urgent or threatening language.
- Requests for sensitive information.
- Suspicious link or shortened URL.

**Checklist warning score:** 7/10

**Assessment:** These warning signs indicate possible risk, not proof of phishing.

**Recommended action:** Verify the message using the bank's official app, manually entered website, or officially published contact details.

## 🚀 Running the Project

### Live Application

Visit:

https://adi-bugata.github.io/PhishGuard-AI-LLM/

### Running from GitHub

1. Open this repository.
2. Open `index.html`.
3. Download or clone the repository if you want to run it locally.
4. Open the application through a local web server or GitHub Pages.

The browser needs an internet connection to load the required JavaScript library and model files. The AI inference itself runs in the browser.

## ⚠️ Limitations

- The application is an educational first-check tool, not a complete phishing detection system.
- The warning score is heuristic and is not a probability of phishing.
- AI-generated explanations may occasionally be inaccurate or incomplete.
- The application does not inspect the actual destination of links.
- It does not verify sender identity or authenticate messages.
- A legitimate message may contain some warning patterns, and a phishing message may avoid them.
- Model performance depends on the user's browser, device, and available resources.

**Important:** Never share passwords, OTPs, banking details, or private messages. Do not click suspicious links to test them.

## 🔮 Future Improvements

- Improved detection of suspicious message patterns.
- Support for additional languages.
- Better explanation quality and consistency.
- More comprehensive testing with different message types.
- Improved accessibility and user experience.
- Additional educational resources about phishing prevention.

## 🎯 Project Goal

The goal of PhishGuard AI is to promote cybersecurity awareness and help users think carefully before trusting suspicious digital messages.

**Think Before You Click. Stay Alert. Stay Safe.**

---

*PhishGuard AI – An educational cybersecurity project.*
