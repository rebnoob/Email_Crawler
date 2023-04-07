#**University Career Service Email Scraper**
This is a Python script that scrapes career service emails of universities from their respective websites. It uses the Selenium library to load the web pages, and the BeautifulSoup library to parse the HTML source code of the web pages.

##**Installation**
Before running the script, you need to install the following dependencies:

selenium
beautifulsoup4
pandas
numpy
requests
You can install them by running the following command:
```python
!pip install selenium beautifulsoup4 pandas numpy requests
```
In addition, you need to install the geckodriver for Firefox, which is used by Selenium to simulate the Firefox browser. You can install it by running the following command:
```python
!apt-get update
!apt install firefox-geckodriver
!cp /usr/lib/geckodriver /usr/bin
!cp /usr/lib/firefox /usr/bin
```
##**Usage**
To use the script, you need to provide a list of university URLs in the list variable, and run the getEmail function for each URL. The getEmail function returns an array of email addresses found on the web page.

You can also use the getLink function to get the first search result link from a Google search for a specific term and university name.

To automate the process of getting the links, you can use the appendLink function to append the search link for each university in a dataframe.

Finally, the getEmailfromLink function retrieves the email addresses from the links in the dataframe, and the resulting 2D array is converted into an array of strings and appended to a list. The final output is a CSV file with the university name, link, and career service emails.

##**Limitations**
The script relies on the HTML structure of the web pages, which may change over time. In addition, some web pages may use dynamic content loading, which may require additional code to scrape.

##**License**
This script is licensed under the MIT License.
