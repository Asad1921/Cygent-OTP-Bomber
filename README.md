Cygent OTPbomber 💣

Overview
Cygent OTPbomber is a tool designed to send multiple OTP (One-Time Password) messages to specified phone numbers, primarily for testing purposes. With enhanced features, it now supports sending OTPs to multiple numbers (via command line or file input) and allows customizable rounds of OTP sends with delays to manage rate limits. This tool is lightweight, user-friendly, and built for educational use.
⚠️ Disclaimer: This tool is intended for educational purposes only. Misuse to harass or harm individuals is strictly prohibited. Always adhere to ethical guidelines, local laws, and obtain explicit permission before testing on any phone number.

Features

Send OTP messages to one or multiple phone numbers in a single run.
Support for input via command line or a text file containing phone numbers.
Configurable rounds of OTP sends per number (e.g., repeat 5 times).
Adjustable delay between rounds to avoid rate limits.
Option to test a single website or all available websites.
Simple command-line interface with progress tracking.
Lightweight and compatible with Python 3.10+.


Prerequisites
Ensure the following are installed on your system:

Python 3.10 or higher
Git (for cloning the repository)
A virtual environment is recommended to manage dependencies safely


Installation
Follow these steps to set up Cygent OTPbomber:

Clone the repository:
git clone https://github.com/Asad1921/Cygent-OTP-Bomber.git
cd Cygent-OTP-Bomber


Create a virtual environment (recommended):
python3 -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate


Install required libraries:Run the following command to install all dependencies listed in requirements.txt:
pip install -r requirements.txt




Usage
Once installed, you can use Cygent OTPbomber with various options to send OTPs to one or more phone numbers. Ensure phone numbers are in the correct format with the country code (e.g., +92 for Pakistan).
Basic Usage
Send OTPs to a single phone number:
python3 core.py +923001234567

Multiple Phone Numbers
Send OTPs to multiple numbers directly:
python3 core.py +923001234567 +923008186777

Input from File
Use a text file (e.g., phones.txt) with one phone number per line:
python3 core.py --file phones.txt

Example phones.txt:
+923001234567
+923008186777

Multiple Rounds
Repeat OTP sends multiple times per number (e.g., 3 rounds):
python3 core.py +923001234567 --rounds 3

Delay Between Rounds
Add a delay (in seconds) between rounds to reduce rate limits:
python3 core.py +923001234567 --rounds 3 --delay 5

Single Website
Test a specific website (e.g., priceoye):
python3 core.py +923001234567 --site priceoye

Combined Example
Send OTPs to multiple numbers from a file and command line, with 2 rounds and a 10-second delay:
python3 core.py +923001234567 --file phones.txt --rounds 2 --delay 10

Disable Clear Screen
Prevent clearing the terminal between runs:
python3 core.py +923001234567 --no-clear




Legal Disclaimer
Cygent OTPbomber is designed for educational purposes only and should not be used for illegal activities, such as spamming or harassing individuals. The developer is not responsible for any misuse of this tool. Always obtain explicit permission before testing on any phone number and comply with local regulations and service terms.

Contribution
Contributions are welcome! To contribute:

Submit a pull request with new features, bug fixes, or additional website modules.
Open an issue to report bugs or suggest improvements.
Ensure code follows the repository’s structure and includes clear documentation.


License
This project is licensed under the MIT License. See the LICENSE file for more details.

