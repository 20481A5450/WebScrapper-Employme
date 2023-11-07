# LinkedIn Job Scraper

This Python script uses Selenium to scrape job listings from LinkedIn without the need for login credentials. It navigates to a specified LinkedIn job search page, scrapes job data, and stores it in a CSV file.

## Prerequisites

Make sure you have Python, Selenium, ChromeDriver, and the Chrome web browser installed. You can install the necessary Python packages using pip:

```
pip install selenium webdriver-manager
```

## Usage instructions:

1. Clone the repository or download the script.

2. Edit the script to specify your LinkedIn job search URL. You can change the `linkedin_url` variable in the script to the desired URL.

3. Open a terminal or command prompt and navigate to the directory where your Python script is located.

4. Make sure you have all the necessary packages and dependencies installed. If you haven't installed them, you can install them using `pip`:

   ```
   pip install selenium webdriver-manager
   ```

5. Start a Jupyter Notebook server by running the following command:

   ```
   jupyter notebook
   ```

6. In your web browser, open the Jupyter Notebook interface by navigating to the URL provided in the terminal, usually something like `http://localhost:8888`.

7. Use the Jupyter Notebook interface to open your `linkedinjobspython.ipynb` script. 

8. Run the script from within the Jupyter Notebook.

## Customization

You can customize the script by changing the following variables:

- `linkedin_url`: Set this to your LinkedIn job search URL.
- `job_cards[:100]`: Adjust the number (100) to limit the number of job postings to scrape.

## Output

The script will generate a CSV file (`linkedin_jobs.csv`) containing job data with the following columns:

- Job Title
- Company
- Location
- Job Link

## Common Errors

1. If you encounter other errors or issues, make sure your ChromeDriver version is compatible with your Chrome browser.

2. `AttributeError: 'NoneType' object has no attribute 'split'`: This error may occur if the LinkedIn page structure changes. Please verify that the CSS selectors used in the script match the current page structure.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments

- Thanks to the [Selenium](https://selenium.dev/) and [WebDriver Manager](https://github.com/SergeyPirogov/webdriver_manager) teams for their valuable tools.

