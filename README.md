# Top-Names.info-Scraper

This Python script is designed to scrape and extract a list of top names from the top-names.info website. It utilizes two key libraries: `requests` and `re`.

## Script Overview

### Data Retrieval
The script makes an HTTP GET request to the specified URL of the top-names.info website using the `requests` library. This fetches the HTML content of the page.

### HTML Parsing
It then processes the HTML content using the `re` library, which is used for regular expression operations. This allows for flexible searching and extraction of data from the HTML content.

### Data Extraction
The script locates the section of the page that contains the list of top names. It extracts these names from the relevant HTML elements using regular expressions and prints them to the console.

### Data Export
Additionally, the script exports the extracted list of names as a JSON file, allowing for easy data storage and further use.

## How It Works

1. **Request Handling:** The script starts by sending a request to the top-names.info URL to get the page content.
2. **HTML Parsing:** Once the content is retrieved, `re` is used to process the HTML and find the section where the names are listed.
3. **Name Extraction:** It identifies and extracts each name using regular expressions to match the specified HTML tags and classes.
4. **Output:** The script outputs the list of top names, each printed on a new line. The names are also saved in a JSON file for convenient storage and retrieval.

## Requirements

- `requests`
- `re` (part of the Python standard library)

You can install the required library using pip:

```bash
pip install requests
```

## Usage

1. **Clone the Repository:**

    ```bash
    git clone https://github.com/Mf4Tn/Top-Names.info-Scraper.git
    ```

2. **Navigate to the Project Directory:**

    ```bash
    cd Top-Names.info-Scraper
    ```

3. **Install the Required Libraries:**

    ```bash
    pip install requests
    ```

4. **Run the Script:**

    ```bash
    python scraper.py
    ```

The extracted names will be printed to the console and saved in a `names.json` file.

