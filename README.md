# 🔒 Password Breach Checker
![GitHub Pages](https://img.shields.io/badge/GitHub%20Pages-Deployed-success?style=flat-square&logo=github)
![License](https://img.shields.io/github/license/Hhhpraise/hhhpraise.github.io?style=flat-square)
![Last Commit](https://img.shields.io/github/last-commit/Hhhpraise/hhhpraise.github.io?style=flat-square)

A secure web application that checks if your password has been compromised in known data breaches, using the Have I Been Pwned API.



## 🌟 Features

- **100% Client-Side Processing** - Your password never leaves your browser
- **Secure Hashing** - Uses SHA-1 hashing before any network request
- **k-Anonymity Model** - Only first 5 characters of the hash are transmitted
- **Detailed Risk Assessment** - Classifies results as Safe, Low, Medium, or High risk
- **Password Education** - Includes security tips and breach statistics
- **Responsive Design** - Works perfectly on all devices
- **No Tracking** - Zero analytics, zero cookies

## 🛠️ How It Works

1. You enter a password in the input field
2. The browser hashes it locally using SHA-1
3. Only the first 5 characters of the hash are sent to the HIBP API
4. The API returns a list of matching hash suffixes with breach counts
5. The application shows you the results with security recommendations

```mermaid
graph TD
    A[User Enters Password] --> B[Client-Side SHA-1 Hashing]
    B --> C[Send First 5 Hash Chars to API]
    C --> D[Receive Matching Hashes]
    D --> E[Display Breach Count & Risk Level]