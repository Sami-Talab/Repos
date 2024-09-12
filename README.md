# Location Based Tax Calculation and Validation Tool

## Description: Features and Purposes 
Jupyter notebook that includes a tool designed to calculate sales tax and validate VAT numbers based on a user's geographical location. Utilizing IP and Tax APIs, the feature determines the user's location through their public IP address, retrieves applicable tax rates (both U.S. and international), and validates VAT numbers for businesses across different countries. 

The primary purpose of this tool is to automate the retrieval of reliable and updated tax information, allowing:
* calculation of correct sales tax for a given product based on location.
* Validation of VAT numbers to ensure compliance with local tax laws.

## APIs used:
1. [IPify API](https://www.ipify.org/): automatically retrieves the user's IP address without asking for input.
  
2. [IPstack API](https://ipstack.com/): gets the geographical details based on the IP address obtained from IPify API. For US based locations, it extract the state code. For international locations, it extracts the country code.
   
3. [Tax Data API](https://apilayer.com/marketplace/tax_data-api): gets the State/country code and displays the latest tax amounts. Allows for the validation of tax numbers and dsiplays relevant results.

## Setup Prerequisites:
API keys for:
* [IPstack API](https://ipstack.com/) 
* [Tax Data API](https://apilayer.com/marketplace/tax_data-api)

## How to use:
1. Choose an option from the main menu:
  * Option 1: Automatically retrieve and display tax rates based on the user's current location.
  * Option 2: Validate a VAT number by providing the VAT number and country code.
  * Option 3: Exit the program.
2. For Option 1:
  * The program will get the public IP address, retrieve location information, and display tax rates (state, city, and combined tax rates) for U.S. locations or global tax rates for non-U.S. locations.
  * Input a product price to calculate the total price with tax.
3. For Option 2:
  * Enter the country code and VAT number for validation.
  * The program will return the validation result, including business name and address, if available.
4. For Option 3:
  * The program terminates.
   

