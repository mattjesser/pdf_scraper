# pdf_scraper
### Extract data from tables in large PDF files
Wrapping the PDFMiner library in some useful functions to make it easier to parse PDF files
This script takes a PDF file and set of pages and creates logs & a dataframe output:
Params:
- base_path = filepath to PDF
- filename = the specific file (without '.pdf')
- pg = desired start page and end page

- 

Five core functions exist:
- pgprep - Returns a list of all the pages you want to parse so you can iterate through them
- pdf_analyze - returns a 'layout' object from PDFMiner for the desired file/page
- extract_data - converts the 'layout' object from PDFMiner into a useable dictionary
- create_logs - returns a summary & detailed view of how PDFMiner reads the page. Use this to adjust your 'prm' variables.
- create_data - returns a final dataframe of the parsed page given the 'out' variables

### Dependencies
pdfminer3
pandas
os
re


