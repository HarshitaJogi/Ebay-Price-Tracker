# eBay Price Tracker
This project is a simple eBay price tracker implemented in Python. It allows you to retrieve and analyze prices of a specific product on eBay, perform data analysis, and predict future prices using a linear regression model. The project utilizes web scraping techniques, data manipulation, and machine learning algorithms.

## Table of Contents
- Dependencies
- Installation
- Usage
- Functionality
- Data Backup and Restoration
- Contributing
- License

## Dependencies
- The following dependencies are required to run the eBay Price Tracker:
- BeautifulSoup
- requests
- numpy
- csv
- scikit-learn

## Installation

1. Clone the repository to your local machine:

   ```
   git clone https://github.com/your-username/ebay-price-tracker.git
   ```

2. Install the required dependencies using pip:

   ```
   pip install -r requirements.txt
   ```

## Usage
1. Open the `ebay_price_tracker.py` file in a Python IDE or editor.
2. Modify the LINK variable to specify the eBay search URL for the desired product. Make sure the URL is in the correct format.

3. Run the script:

   ```
   python ebay_price_tracker.py
   ```

## Functionality
The eBay Price Tracker provides the following functionality:

1. Retrieving prices from the specified eBay search URL using web scraping techniques.
2. Removing outliers from the price data.
3. Calculating the average price of the product.
4. Saving the average price with the current date to a CSV file.
5. Training a linear regression model to predict future prices based on the historical price data.
6. Predicting prices for the next `n` days using the trained model.
7. Backing up the price data to a separate CSV file.
8. Restoring the price data from the backup file.

## Data Backup and Restoration
The eBay Price Tracker allows you to backup and restore the price data to prevent data loss.

- To backup the data, use the `backup_data()` function. It will create a backup file named `data_backup.csv`.
- To restore the data from the backup file, use the `restore_data()` function. It will restore the data from `data_backup.csv` if it exists.

Note: It's recommended to regularly backup the data to avoid losing any important price records.

## Contributing
Contributions to this project are welcome. If you find any issues or have suggestions for improvements, please open an issue or submit a pull request.

When contributing, please follow the existing code style and ensure that your changes are well-documented and tested.

## License
Feel free to use, modify, and distribute the code for personal or commercial purposes.

