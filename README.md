# Currency_Converter-Introduction to Programming Project

## Overview
This is a Python-based desktop application for currency conversion with GUI, designed to make life easier by avoiding the hassle of navigating through complex financial websites. The tool uses the ExchangeRate-API to provide real-time data and has a resilient architecture that embeds tkinter in the frontend, while the requests library is used for backend operations, ensuring functionality even without an internet connection through an intelligent offline caching system.

## Features
** Real-time data fetching:** Fetches real-time exchange rates for USD, INR, EUR, etc., using a live REST API.
**Resilient Offline Mode:** Automatically switches to a fallback local dataset if network error conditions are detected.
**Input Validation:** Provides error handling for non-numeric inputs that prevents application crashes.
**User-Friendly GUI:** Clean interface with drop-down menus for selecting currencies and clear results display.
**Cross-Platform Compatibility:** Because it's Python-based, this application will run on any system that has a working Python environment in place, be it Windows, macOS, or Linux.
## Technologies/Tools Used
**Programming Language: ** Python 3.7
**GUI Framework: ** Tkinter
**HTTP Library: ** Requests (for API calls)
**Data Format: ** JSON
**API Service: ** ExchangeRate-API
##Steps to install and run the program
## Steps to Install & Run the Project

1.  *requirement:*
Make sure that Python is installed on your system. You can check this by running the following:
bash
     python -->version 3.7
2.  *Clone/Download the Repository:*
Download the project files to your local machine.
3.  *Install Dependencies:*
This project requires the requests library. In your terminal or command prompt, run the following:
bash
     pip install requests
4.  *Run the Application:*
Go to your project directory and run the script:
 bash
      python Currency_Converter.py
## Instructions for testing
Conduct the following tests to ensure that the application works as anticipated.

1.  *Standard Conversion Test:
* Launch the app.
* In the Amount field, enter "100".
Select "INR" as the From currency and "USD" as the To currency.
* Click "Convert Now."

* Expected Output: The result of a calculation is shown at the end. Example: "Result: 1.2 USD"
2.  *Input Validation Test:*
* Launch the application.
* Type in any string or leave the Amount field blank.

* Click "Convert Now."
* Expected Output: A warning pop-up showing "Please enter a valid numeric amount" or "Please enter an amount."
3.  Offline/Network Error Test:
* Disconnect your computer from the internet. * Restart the application. * Expected Output: The app should print a "Network Error" error message but still open. * Try converting USD to EUR or to INR. It should work using the hardcoded fallback rates.
## Project structure
# currency converter
 ├── currency_converter.py
 ├── README.md
 ├── Report.pdf
 ├── /screenshots
 └── /recordings
