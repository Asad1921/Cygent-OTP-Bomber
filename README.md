# Cygent OTP Bomber 💣
![](<img width="1024" height="1024" alt="image" src="https://github.com/user-attachments/assets/931a3d9e-e85f-407c-8f6a-8d5a568b54a8" />
)

## Overview

Cygent OTPbomber is a tool designed to send multiple OTP (One-Time Password) messages to specified phone numbers, primarily for testing purposes. With enhanced features, it now supports sending OTPs to multiple numbers (via command line or file input) and allows customizable rounds of OTP sends with delays to manage rate limits. This tool is lightweight, user-friendly, and built for educational use.

⚠️ **Disclaimer**: This tool is intended for educational purposes only. The misuse of this tool to harass or harm individuals is strictly prohibited. Please adhere to ethical guidelines and local laws.

---

## Features

- Send 100+ OTP messages to a specified number within a minute.
- Simple and user-friendly command-line interface.
- Lightweight and easy to install on any machine running Python.

---

## Prerequisites

To use this tool, ensure you have the following installed:

- Python 3.10 or higher
- Git (for cloning the repository)
- A virtual environment is recommended to manage dependencies safely

---

## Installation

Follow these steps to download and set up the tool:

1. **First of all you have to create a virtual environment then you will clone repository, For now run below commands in your linux(ANY) terminal**:
   ```bash
   python3 -m venv venv
   ```
   ```bash
   source venv/bin/activate
   ```
   ```bash
   unset http_proxy https_proxy HTTP_PROXY HTTPS_PROXY
   ```
2. **Clone the repository**:
   ```bash
   git clone https://github.com/Asad1921/Cygent-OTP-Bomber.git
   mv Cygent-OTP-Bomber otpbomber
   cd otpbomber
   ```

3. **Install required libraries**:
   Run the following command to install all dependencies.
   ```bash
   pip install -r requirements.txt
   ```


---

## Usage

Once installed, you can use Cygent OTPbomber with various options to send OTPs to one or more phone numbers. Ensure phone numbers are in the correct format with the country code (e.g., +92 for Pakistan).
Basic Usage
Send OTPs to a single phone number:

# python3 core.py +923001234567

Multiple Phone Numbers
Send OTPs to multiple numbers directly:
# python3 core.py +923001234567 +923009186777

Input from File
Use a text file (e.g., phones.txt) with one phone number per line:
# python3 core.py --file phones.txt

Example phones.txt:
+923001234567
+923008186777

Multiple Rounds
Repeat OTP sends multiple times per number (e.g., 3 rounds):
# python3 core.py +923001234567 --rounds 3

Delay Between Rounds
Add a delay (in seconds) between rounds to reduce rate limits:
# python3 core.py +923001234567 --rounds 3 --delay 5

Single Website
Test a specific website (e.g., priceoye):
# python3 core.py +923001234567 --site priceoye

Combined Example
Send OTPs to multiple numbers from a file and command line, with 2 rounds and a 10-second delay:
# python3 core.py +923001234567 --file phones.txt --rounds 2 --delay 10

Disable Clear Screen
Prevent clearing the terminal between runs:
python3 core.py +923001234567 --no-clear

## Legal Disclaimer

This tool is designed for **educational purposes** only and should not be used for illegal activities. The developer is not responsible for any misuse of this tool. Please be mindful of local regulations and ethical guidelines when using such tools.

---

## Contribution

If you would like to contribute to this project, feel free to submit a pull request or open an issue in the repository. We welcome all suggestions and improvements.

---

## License

This project is licensed under the MIT License. See the `LICENSE` file for more details.

---
