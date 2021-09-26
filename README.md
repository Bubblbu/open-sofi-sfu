# Open SOFI - SFU

> Opening the Statements of Financial Information provided by Simon Fraser University.

This is an experimental project to provide [SFU's financial information](https://www.sfu.ca/finance/publications.html) in an open and accessible way.

Initial proposed workflow:

1. Extract data from respective PDFs published each year (mostly manual effort reyling on PDF extraction tools)
2. Automaticall clean and transform data using python (`pandas`)
3. Load data into SQLITE database (`pandas` & `sqlite-utils`)
4. Publish data using [datasette](https://datasette.io/)