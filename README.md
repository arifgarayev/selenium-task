# Selenium WebDriver - Python home task

You need to automate the process of scraping product details (product name, price, and rating) from an `amazon.com` using Chrome WebDriver and Python. Implement Page Object Model (POM) design pattern and Xpath locators to extract the required data from the website.

### Steps

1. Open the Chrome browser using the Chrome WebDriver.
2. Navigate to the `amazon.com` website.
3. Search for any product using the search bar.
4. Click on the first product in the search results to open the product page.
5. Extract the product name, price, and rating using Xpath locators and store them in a dictionary object.
6. Click on the "next" button to navigate to the next product page and repeat step 5 until all products on the page have been scraped.
7. Click on the "next" button again to navigate to the next page and repeat step 5 and 6 until all pages have been scraped.
8. Save the scraped data to a CSV file (requirements: pandas)

# Design

The following base classes should be implemented using POM design pattern. You can add as many classes as you want.

1. HomePage class: This class should contain methods to navigate to the website, enter the search query and submit the search.
2. SearchResultPage class: This class should contain methods to click on the first search result and navigate to the product page.
3. ProductPage class: This class should contain methods to extract the product details (product name, price, and rating) using Xpath locators and store them in a dictionary object.
4. Main class - entrypoint: This class should contain the main function to instantiate the classes and call the methods to perform the automation task.
5. Scenarios class: This class should contain different scenarios for different occasions/unexpected errors.
6. You may implement other design patterns (factory method for example).
7. Make you project well structured (folder/dependency structure), more readble and extendable. Strictly follow SOLID principles.

## Challenges

Here are some challenges that can be encountered during this task

1. Identifying the correct Xpath locators to extract the required data.
2. Handling dynamic Xpath locators that change every time the page is loaded.
3. Handling pop-up windows that appear during the automation process.
4. Implementing proper error handling to handle exceptions and errors during the automation process.
5. Ensuring that the automation process is robust and can handle edge cases, such as invalid search queries or missing data on product pages.
6. Assume that your project will run 24/7. You might want to use some sort of proxy to bypass network IP blocks and make your script runnable infinately, even there is an error occured.

## Grading

- Project fully functional and meets requirements: **50%**
- Git usage: **10%**
- Complexity, readability, scalability, comments (English only), and implementing best-practices: **20%**
- Following any OO design pattern: **20%**

## Useful links

- [OOP design patterns](https://python-patterns.guide)
