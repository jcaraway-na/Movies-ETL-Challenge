# Movies-ETL-Challenge

## BACKGROUND

> Amazing Prime loves the dataset and wants to keep it updated on a daily basis. Britta needs your help to create an automated pipeline that takes in new data, performs the appropriate transformations, and loads the data into existing tables. You’ll need to refactor the code from this module to create one function that takes in the three files—Wikipedia data, Kaggle metadata, and the MovieLens rating data—and performs the ETL process by adding the data to a PostgreSQL database.

### OBJECTIVE

>This new assignment consists of two technical analysis deliverables and a written report to present your results. 
> You will submit the following:

- Deliverable 1: Write an ETL Function to Read Three Data Files
- Deliverable 2: Extract and Transform the Wikipedia Data
- Deliverable 3: Extract and Transform the Kaggle data
- Deliverable 4: Create the Movie Database

---

### Deliverable 1: Write an ETL Function to Read Three Data Files

<table>
  <tr>
    <td>Complete</td>
    <td>Task</td>
    <td>Example</td>
  </tr>
  <tr>
    <td> :white_check_mark: </td>
    <td> 1.) The ETL function is written to read in the three data files.</td>
    <td><img src="https://github.com/jcaraway-na/Movies-ETL-Challenge/blob/main/resources/read_in_three_data_files.png" width=100% height=100%></td>
  </tr>
  <tr>
    <td> :white_check_mark: </td>
    <td> 2.) The function converts the Wikipedia JSON file to a Pandas DataFrame, and the DataFrame is displayed in the ETL_function_test.ipynb file. </td>
    <td><img src="https://github.com/jcaraway-na/Movies-ETL-Challenge/blob/main/resources/wiki_movies_df.png" width=100% height=100%></td>
  </tr>
  <tr>
    <td> :white_check_mark: </td>
    <td> 3.) The function converts the Kaggle metadata file to a Pandas DataFrame, and the DataFrame is displayed in the ETL_function_test.ipynb file. </td>
    <td><img src="https://github.com/jcaraway-na/Movies-ETL-Challenge/blob/main/resources/kaggle_metadata_df.png" width=100% height=100%></td>
  </tr>
  <tr>
    <td> :white_check_mark: </td>
    <td> 4.) The function converts the MovieLens ratings data file to a Pandas DataFrame, and the DataFrame is displayed in the ETL_function_test.ipynb file. </td>
    <td><img src="https://github.com/jcaraway-na/Movies-ETL-Challenge/blob/main/resources/ratings_df.png" width=100% height=100%></td>
  </tr>
</table>

---

### Deliverable 2: Extract and Transform the Wikipedia Data

<table>
  <tr>
    <td>Complete</td>
    <td>Task</td>
    <td>Example</td>
  </tr>
  <tr>
    <td> :white_check_mark: </td>
    <td> 1.) The TV shows are filtered out, and the wiki_movies_df DataFrame is created.</td>
    <td><img src="https://github.com/jcaraway-na/Movies-ETL-Challenge/blob/main/resources/filter_out_tv_shows.png" width=100% height=100%></td>
  </tr>
  <tr>
    <td> :white_check_mark: </td>
    <td> 2.) A try-except block is used to catch errors while extracting the IMDb IDs with a regular expression and dropping duplicate IDs. </td>
    <td><img src="https://github.com/jcaraway-na/Movies-ETL-Challenge/blob/main/resources/IMDb_try_except.png" width=100% height=100%></td>
  </tr>
  <tr>
    <td> :white_check_mark: </td>
    <td> 3.) The extraction and transformation of the Wikipedia data in the ETL function does the following:
        <p> A list comprehension is used to keep columns with non-null values.</p>
        <p> The non-null box office data is converted to string values using the lambda and join functions.</p>
        <p> A regular expression is used to match the six elements of "form_one" of the box office data.</p>
        <p> A regular expression is used to match the three elements of "form_two" of the box office data.</p>
        <p> The following columns are cleaned in the Wikipedia DataFrame:</p>
        <li> - The box office column</li>
        <li> - The budget column</li>
        <li> - The release date column</li>
        <li> - The running time column</li>
      <p> </p>
      <p> The cleaned Wikipedia data is converted to a Pandas DataFrame, and the DataFrame is displayed in the ETL_clean_wiki_movies.ipynb file.</p>
    </td>
    <td>
      <img src="https://github.com/jcaraway-na/Movies-ETL-Challenge/blob/main/resources/list_comprehension_non-null_values.png" width=100% height=100%>
      <img src="https://github.com/jcaraway-na/Movies-ETL-Challenge/blob/main/resources/six_from-one_three_from-one.png" width=100% height=100%>
      <img src="https://github.com/jcaraway-na/Movies-ETL-Challenge/blob/main/resources/clean_columns.png" width=100% height=100%>
      <img src="https://github.com/jcaraway-na/Movies-ETL-Challenge/blob/main/resources/clean_wiki.png" width=100% height=100%>
    </td>
  </tr>
</table>
