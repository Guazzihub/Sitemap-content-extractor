# Sitemap Content Extractor

This Python script extracts text content from web pages listed in an XML sitemap and generates a Word document (`.docx`) with the extracted content. It uses `requests`, `BeautifulSoup`, and `python-docx` for web scraping and document creation.

## Features

- Parses an XML sitemap to extract URLs.
- Scrapes text content from each webpage.
- Removes unnecessary elements like scripts and styles.
- Generates a clean and structured Word document with headings for each URL.

## Requirements

You can install all dependencies using the following command:

```bash
pip install -r requirements.txt
```

## How to Use

1. Clone the repository or download the script.
2. Install the required dependencies using the command mentioned earlier.
3. Update the `sitemap_url` variable in the script to point to the desired sitemap XML URL.
4. Run the script:

   ```bash
   python app.py
   ```

## File Structure

```
.
├── app.py          # The main Python script
├── requirements.txt        # Dependencies
└── site_content.docx       # Output Word document
```

## Example

To use the script with the sitemap URL `http://example.com/sitemap.xml`, update the following line in the script:

```python
sitemap_url = 'http://example.com/sitemap.xml'
```

After running the script, the extracted content will be saved in `site_content.docx`.

## Notes

- Ensure the sitemap XML is accessible and follows the standard format.
- Large websites with extensive sitemaps may take longer to process.
