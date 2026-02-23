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

---

## Lab Challenge: Data Wrangling with the Netflix Dataset (Kaggle)

### Problem Statement

The goal of this lab challenge was to develop hands-on experience in data wrangling using a real-world dataset sourced from Kaggle and to publish the cleaned results on the Kaggle platform. The assignment focused on cleaning, structuring, transforming, and validating the Netflix Movies and TV Shows dataset to ensure it was suitable for accurate analysis and visualization.

The dataset used in this challenge was obtained from Kaggle:  
https://www.kaggle.com/datasets/shivamb/netflix-shows

---

### Approach

The task began by loading the Netflix dataset from a CSV file into a pandas DataFrame within a Kaggle Notebook environment. Initial data discovery was conducted to understand the dataset’s structure, including its dimensions, column data types, missing values, and duplicate records.

Next, the dataset was structured and transformed by converting date fields into proper datetime formats and decomposing complex fields such as duration into separate numeric and categorical components. Additional formatting improvements were applied to enhance consistency across columns.

The cleaning phase involved removing duplicate records, dropping unnecessary columns, and handling missing values. Missing director and country fields were intelligently imputed using inferred relationships between directors, cast members, and country information, while remaining null values were assigned a standard placeholder to preserve dataset integrity. Rows with critical missing information were removed where appropriate.

Data validation checks were then performed to identify logical inconsistencies, such as content being added to Netflix before its release year. The dataset was reviewed for completeness, correctness of data types, and overall consistency. Temporary columns created during wrangling were removed, the index was reset, and random samples were inspected to confirm accuracy.

Finally, the cleaned and validated dataset was exported as a CSV file and prepared for publication on Kaggle.

---

### Tools Used

- **Python** for data manipulation and cleaning  
- **Kaggle Notebooks** as the execution and publishing environment  
- **Pandas** for data loading, exploration, transformation, and validation  
- **Datetime utilities** for temporal validation and consistency checks  

---

### Key Lessons Learned

This lab reinforced the importance of systematic data discovery before cleaning and transformation. It demonstrated practical techniques for handling missing values using domain logic rather than simple deletion, as well as the value of validating datasets using real-world constraints. The assignment also strengthened proficiency in pandas for end-to-end data wrangling workflows and highlighted best practices for preparing high-quality datasets ready for analysis, visualization, and publication.
