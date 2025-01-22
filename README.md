# web-scraper-to-mysql
A Python project that scrapes SMM panel service data from multiple websites, stores the information in a MySQL database, and exports the results to a CSV file. This tool is helpful for analyzing services from platforms like LikesOutlet, GodOfPanel, Followiz, and SMMBind.

## Description
A Python project that scrapes SMM panel service data from multiple websites, stores the information in a MySQL database, and exports the results to a CSV file. This tool is helpful for analyzing services from platforms like LikesOutlet, GodOfPanel, Followiz, and SMMBind.
## Features
+ Scrapes service details from multiple SMM panel websites.
+ Saves scraped data into a MySQL database for further analysis.
+ Exports combined data into a CSV file for easy access and use.
## Contribution
Contributions are welcome! Please fork this repository, make your changes, and submit a pull request.
this repo was make with the contribution of 
+ abeselomsolomongetahun@gmail.com

## Usage
### Clone the Repository
git clone https://github.com/your-username/web-scraper-to-mysql.git
cd web-scraper-to-mysql
# Python Dependencies
Include the following dependencies in your requirements.txt file to ensure users can easily set up the environment:
+ requests
+ beautifulsoup4
+ mysql-connector-python
### Install Dependencies
Use pip to install the required libraries:

+ pip install -r requirements.txt
## Export Data
+ The script will generate a CSV file named services_combined.csv with the scraped data.

## Run the Script
Execute the script to scrape data and store it in the database:
+ python app.py
## Set Up the MySQL Database
Create a MySQL database and a table with the following structure:
```bash
CREATE TABLE services (
    service_id VARCHAR(255),
    service_name VARCHAR(255),
    rate_per_thousand VARCHAR(255),
    min_quantity VARCHAR(255),
    max_quantity VARCHAR(255),
    avg_time VARCHAR(255),
    category VARCHAR(255),
    details TEXT,
    provider VARCHAR(255)
);
// Update the database credentials in the connect_to_database function:


mysql.connector.connect(
    host='your_host',
    user='your_username',
    password='your_password',
    database='your_database'
)








