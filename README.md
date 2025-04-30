# Instagram Reporter Bot

This project automates the process of reporting an Instagram account through a script using Python and Selenium.

---

## Features
- **Automated Login**: Logs into Instagram using credentials from a configuration file.
- **Automated Reporting**: Navigates through the interface to report a specified user account.
- **Configurable Settings**: User credentials are loaded from a JSON configuration file for easy updates.

---

## Requirements
To use this script, ensure you have the following installed on your system:
1. Python 3.8 or later
2. Google Chrome browser
3. ChromeDriver (compatible with your Chrome version)

---

## Installation

### 1. Download the Repository

- Download the project to your computer.

### 2. Install Dependencies
Install the required Python libraries using pip:
```bash
pip install -r requirements.txt
```

### 3. Configuration
Create a `config.json` file in the project directory with the following structure:
```json
{
  "username": "your_instagram_username",
  "password": "your_instagram_password"
}
```


### 4. Set Up ChromeDriver
Download ChromeDriver from [https://chromedriver.chromium.org/](https://chromedriver.chromium.org/) and ensure it is in your system's PATH or in the project folder.

---

## Usage
### Run the Script
To start the script, execute the following command in your terminal:
```bash
python reporter.py
```

## Media 

https://github.com/user-attachments/assets/8813c21a-04c2-43fb-9653-a5b01c3076e0

### Enter the Username to Report
Once the script starts, you'll be prompted to enter the username of the Instagram account you want to report.

---

## How It Works
1. **Launch Chrome**: The script initializes a Chrome browser instance using Selenium.
2. **Login Process**:
   - Opens the Instagram login page.
   - Inputs the username and password from the `config.json` file.
   - Handles cookies and login prompts automatically.
3. **Reporting Loop**:
   - Navigates to the target user's profile.
   - Automates the reporting process by simulating user interactions.
   - Loops the reporting action continuously.

---

## Warnings
- **Ethical Use**: This script is for educational purposes only. Misusing this script to harm or harass others violates Instagram’s policies and may have legal consequences.
- **Liability**: The author of this script is not responsible for any misuse or resulting consequences.

---

## Troubleshooting

### Common Errors
1. **ElementNotInteractableException**: Ensure the XPaths in the script match Instagram's current DOM structure. Instagram's interface may update, requiring you to adjust the XPaths.
2. **WebDriverException**: Confirm that ChromeDriver is compatible with your installed version of Chrome.

### Debugging Tips
- Use the `headless=False` option in the script to visually inspect the browser’s actions.
- Update ChromeDriver and dependencies to their latest versions.

---

## Contributing
Contributions to improve this project are welcome. Feel free to submit a pull request or open an issue for suggestions or bug fixes.

---

## Disclaimer
This project is not affiliated with or endorsed by Instagram. Use at your own risk, and respect the platform's terms and community guidelines.

---

## License
This project is licensed under the [MIT License](LICENSE). 