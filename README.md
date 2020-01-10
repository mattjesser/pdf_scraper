# pdf_scraper
### Extract data from tables in large PDF files
This script creates a function `convert_pdf_to_txt` with two variables:
- path = filepath to PDF
- pg = desired page number

Optionally, you can pass the raw text to a function that parses the text object and puts in a pandas dataframe

### Dependencies
pdfminer3
pandas
io
