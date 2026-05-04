# Chat Translator Automation Testing (ITPM Assignment 1)

This repository contains the automated test scripts using Playwright to evaluate the transliteration accuracy of the Chat Translator application for the IT3040 – ITPM assignment.

## Prerequisites

Before running the tests, ensure you have the following installed on your machine:
- **Python 3.11 or 3.12**
- **pip** (Python package installer)

## Installation

1. **Clone the repository** (or extract the folder):
   ```bash
   git clone <your-repository-url>
   cd IT23833470
   ```

2. **Install the required Python dependencies**:
   ```bash
   pip install -U pip
   pip install playwright openpyxl
   ```

3. **Install Playwright browsers**:
   Run the following command to download the necessary Chromium browser binaries required for Playwright automation:
   ```bash
   python -m playwright install chromium
   ```

## Running the Tests

To execute the automated test cases and record the results into the Excel file, navigate to the folder containing the script and run the following command in your Command Prompt/Terminal:

```bash
python "IT23833470_test_automation.py" --excel "IT23833470_Assignment 1 - Test cases.xlsx" --url "https://www.pixelssuite.com/chat-translator" --wait-ms 5000 --type-delay-ms 80 --slow-mo-ms 200 --save-every 1
```

### Important Notes:
- **Do not open the Excel file** (`IT23833470_Assignment 1 - Test cases.xlsx`) while the tests are running, as it will cause a `Permission Denied` error when the script attempts to save the results.
- The automation will interact with the browser directly. Please do not interrupt the mouse or keyboard inputs while the browser is actively typing the test cases.
- Execution will take approximately 20-25 minutes to complete all test cases. The results will be populated under the **Actual Output** and **Status** columns in the Excel file.
