# A-web-scraping-project-for-books.toscrape.com-using-Python-and-BeautifulSoup
A Python web scraping project for extracting book information from the website http://books.toscrape.com/

This project involves web scraping the Books to Scrape website, which contains a catalog of books. The scraping is done using Python's Requests and BeautifulSoup libraries, and the data is extracted from each book's page on the website. The data includes book titles, descriptions, prices, availability, and image URLs.

The scraped data is then stored in both MySQL and MongoDB databases, and also in CSV files for backup purposes. The project uses Python's pymysql and pymongo libraries for database connections and management.

The project is split into four Jupyter notebooks: one for basic web scraping, one for scraping books by category, one for saving data to CSV and MySQL, and one for saving data to CSV and MongoDB. Each notebook has its own set of functions and code to accomplish its specific task.

Overall, this project demonstrates how to use web scraping techniques to extract useful data from a website, and how to store that data in various types of databases for future use.
## The project includes several functionalities for retrieving and storing book information:

### Part 1: Scraping books by category
The script uses the Python requests library and BeautifulSoup to parse the HTML of each page and extract the book URLs. In this notebook, we specifically focus on scraping books by category, which means we collect information about books based on their respective categories.

### Part 2: Basic web scraping
This part is a web scraping analysis of books.toscrape.com, a website for book lovers. The notebook includes code to extract information such as the number of pages, number of books on each page, total number of books, and the number of books in each category. The data is saved in a CSV file for further analysis.

### Part 3: Saving to CSV and MySQL
The notebook uses the requests library and BeautifulSoup to parse the HTML of each page and extract the book's title, rating, availability, url_slug, and image_url.
The code then saves this information to a CSV file named "data/books_info.csv" and to a MySQL database. The script uses the Python mysql-connector library to connect to the database and insert the data into a table. It checks if the MySQL connection is successful before attempting to save the data to the database.

Overall, this code provides a basic framework for scraping and saving data from this website. It could be modified or expanded to include additional information or features as needed.


### Part 4: Saving to MongoDB
The save_to_mongodb.py script saves the scraped book information to a MongoDB database. The script uses the Python pymongo library to connect to the database and insert the data into a collection. It includes each indivual books title, description, upc, price, availability, and image_url. It also saves to data/books.csv. 

# How to Use
To use this project, clone the repository and run each script in the order specified above. Make sure to set up the appropriate database credentials and connection details in the corresponding scripts.

### How to Use
#### To run the app, first clone the repository:
    git clone https://github.com/actuaryhafeez/A-web-scraping-project-for-books.toscrape.com-using-Python-and-BeautifulSoup.git
#### Next, install the required packages using pip:
    pip install -r requirements.txt
### Run Jupyter Notebook using the following command to open notebook.ipynb
    jupyter notebook

![books](https://user-images.githubusercontent.com/55107467/234138130-26b3692d-75dd-4b0c-9328-e801dc2f3598.png)


## Project Structure 

    A-web-scraping-project-for-books.toscrape.com-using-Python-and-BeautifulSoup/
        ├── data/
        ├── app.py/
        ├── basics.ipynb/
        ├── books_categories.ipynb/
        ├── save to csv and mysql.ipynb/
        ├── save to mongodb.ipynb/
        ├── requirements.txt/
        ├── README.md/

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

This project adheres to the [Open Source Initiative's](https://opensource.org) definition of open source software and the [Open Source Initiative's Approved License List](https://opensource.org/licenses/alphabetical).


# References

### Acknowledgements
This project was built using the following tools and resources:

* Python
* BeautifulSoup
* requests
* http://books.toscrape.com/
