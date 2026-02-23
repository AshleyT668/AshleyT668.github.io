## Lab Challenge: Web Scraping with Python

### Problem Statement

The objective of this lab challenge was to gain practical experience in automating web data collection using Python within a Google Colab (Jupyter Notebook) environment. The task required scraping structured data from a live website and transforming it into a usable dataset. Specifically, the challenge involved extracting tabular hockey statistics from a publicly available webpage and exporting the cleaned data into a CSV file for further analysis.

The target website for the scraping task was:  
https://www.scrapethissite.com/pages/forms/

---

### Approach

The solution followed a step-by-step web scraping workflow. First, an HTTP GET request was sent to the target webpage to retrieve its HTML content. The retrieved page source was then parsed using an HTML parser to allow structured navigation of the document.

Once the HTML content was parsed, the relevant table containing hockey data was located by identifying its HTML class attribute. Column headers were extracted from the table’s `<th>` elements and used to define the structure of a pandas DataFrame. The data rows were then iterated over, with each cell’s text content cleaned and appended row by row to the DataFrame.

After verifying the correctness of the extracted data, the final structured dataset was exported as a `.csv` file, enabling easy storage, sharing, and further analysis.

---

### Tools Used

- **Python** for implementing the scraping logic  
- **Google Colab (Jupyter Notebook)** as the development and execution environment  
- **Requests** to send HTTP requests and retrieve webpage content  
- **BeautifulSoup** to parse and navigate the HTML structure  
- **Pandas** to store, manipulate, and export structured data  

---

### Key Lessons Learned

This lab reinforced the importance of understanding HTML structure when scraping web data and demonstrated how different Python libraries work together in a data collection pipeline. It highlighted best practices in separating concerns between data retrieval, parsing, cleaning, and storage. The exercise also improved familiarity with pandas DataFrames and file export operations, as well as practical experience working in a cloud-based notebook environment. Overall, the challenge strengthened confidence in building end-to-end data extraction workflows using Python.
