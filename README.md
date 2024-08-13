# KeyLogger and System Monitoring Tool
## Overview
This project is a Python-based keylogger and system monitoring tool. It captures keyboard inputs, mouse events, takes screenshots, records audio, and collects system information. The data is periodically sent to an email address.

Important: Use this tool only in legal and ethical scenarios, such as for educational purposes, in environments where you have explicit permission, or as part of a legitimate security testing scenario. Misuse of this tool could lead to serious consequences.

## Features
Keyboard Logging: Records all keystrokes and saves them to a log.
Mouse Tracking: Logs mouse movements, clicks, and scrolls.
System Information: Gathers and logs system details such as hostname, IP address, and operating system.
Audio Recording: Records audio from the microphone and saves it as a WAV file.
Screenshot Capturing: Takes a screenshot of the current screen.
Periodic Reporting: Sends collected data to a specified email address at regular intervals.
## Installation
### Prerequisites
Ensure you have Python installed on your system. You can download it from python.org.

### Dependencies
The script requires the following Python packages:

logging
os
platform
smtplib
socket
threading
wave
pyscreenshot
sounddevice
pynput
email
You can install the necessary packages using pip:

bash
Copy code
pip install pyscreenshot sounddevice pynput
Configuration
Clone this repository:

#### bash
Copy code
git clone https://github.com/your-username/your-repo-name.git
cd your-repo-name
Open the script and update the EMAIL_ADDRESS and EMAIL_PASSWORD with your email credentials.

#### python
Copy code
EMAIL_ADDRESS = "YOUR_USERNAME"
EMAIL_PASSWORD = "YOUR_PASSWORD"
Ensure that the email SMTP server settings are correct. The current settings use Mailtrap for testing.

## Usage
Run the script from the command line:

### bash
Copy code
python your_script_name.py
The script will start logging keystrokes, mouse movements, and system information. It will also periodically send reports via email.

## Notes
Security: This script is intended for educational purposes. Ensure you have explicit permission to run it in any environment.
Email Configuration: Update the email settings according to your email service provider. The current configuration uses Mailtrap for testing.
Platform-Specific Behavior: The script contains platform-specific code for closing and deleting itself. Be cautious and make sure you understand these actions before using it.
## Disclaimer
This script is provided for educational purposes only. Use it responsibly and ensure you have appropriate permissions. Unauthorized use of keyloggers or similar tools is illegal and unethical.

## License
This project is licensed under the MIT License - see the LICENSE file for details.
