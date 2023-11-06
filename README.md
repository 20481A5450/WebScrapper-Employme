# LinkedIn Job Scraper

## Overview

This Python script is designed to scrape job postings from LinkedIn based on a specific search query and save the job data to a CSV file. It uses the Selenium library to automate the web scraping process.

## Requirements

Make sure you have the following packages installed in your Python environment:

- `selenium`
- `webdriver-manager`

You can install them using `pip`:

```bash
pip install selenium webdriver-manager
```

## Usage

1. Import the necessary libraries and set up the Chrome driver with appropriate options and configurations.

2. Provide the LinkedIn job search URL as `linkedin_url`. You can modify the search query by changing the URL.

3. Run the script, which will:

   - Launch a headless Chrome browser.
   - Navigate to the LinkedIn job search page.
   - Collect job data, including job title, company, location, and job link for the first 100 job postings.
   - Save the job data to a CSV file named `linkedin_jobs.csv`.

4. The script will print the number of jobs successfully scraped and saved in the CSV file.

## Sample Output

Here is a sample of the job data saved in the CSV file:

```csv
Job Title,Company,Location,Job Link
Software Engineer,ABC Company,New York,https://www.linkedin.com/jobs/software-engineer-12345
Data Scientist,XYZ Corporation,San Francisco,https://www.linkedin.com/jobs/data-scientist-67890
...
```

## Notes

- The script uses a headless Chrome browser to perform web scraping, ensuring that it doesn't open a visible browser window during the process.
- It limits the scraping to the first 100 job postings, but you can adjust this limit as needed by modifying the `job_cards` loop.

Feel free to customize the script for your specific LinkedIn job scraping needs.

---

You can save the README content to a file named `README.md` and include it in your project repository for clear documentation.
