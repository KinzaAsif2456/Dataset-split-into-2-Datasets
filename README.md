# Splitting by rows
Using Groupby and Disctinary comprehension.
In this Dataset 1 contains 2 companies in  alternative rows , isplit both comapnies and made them as 2 new datastets

## Annual Temperature Data Analysis  

### Overview
The code reads in the annual temperature data from a CSV file named annual_temp.csv. It then uses the groupby method to separate the data by source and creates a dictionary where each key is a source (GCAG or GISTEMP) and each value is the corresponding DataFrame.
The separated data is then saved to new CSV files in the /content/ directory. Finally, the code loads the saved CSV files back into DataFrames and prints out the total number of rows in each dataset.

### File Description
**annual_temp.csv:**  The original dataset containing annual temperature data with a 'Source' column that specifies the source of the data.
**annual_temp_gcag.csv:**  A CSV file containing the subset of data where the 'Source' is 'GCAG'.
**annual_temp_gistemp.csv:**  A CSV file containing the subset of data where the 'Source' is 'GISTEMP'.

### Description  
This project analyzes annual temperature data from two sources: GCAG (Global Climate Analysis Group) and GISTEMP (Goddard Institute for Space Studies Surface Temperature Analysis). The dataset includes mean temperature values from various years, allowing for comparative analysis between the two sources.  

### Features  
- Loads annual temperature data from CSV files.  
- Provides total row counts for the original dataset, GCAG dataset, and GISTEMP dataset.  
- Displays mean temperature values over the years from both sources.  

### Requirements
**pandas:** For data manipulation and CSV file handling.

### Usage
- Clone this repository to your local machine.
- Make sure you have the pandas library installed.
- Run the code using Python (e.g. python annual_temp_processing.py).
- The separated data will be saved to new CSV files in the /content/ directory.
- The script will output the total number of rows in the original dataset and each separated dataset.

### Load the dataset into CSV files  
gg_df = pd.read_csv("/content/annual_temp_gcag.csv")  
gm_df = pd.read_csv("/content/annual_temp_gistemp.csv")  

### Print total rows in the original dataset  
print(f"\nTotal rows in original dataset: {len(gg_df) + len(gm_df)}")  
print(f"Total rows in GCAG dataset: {len(gg_df)}")  
print(f"Total rows in GISTEMP dataset: {len(gm_df)}")  

## Contributing
Contributions are welcome! If you have suggestions for improvements or additional features, please fork the repository and submit a pull request.

## License
This project is licensed under the MIT License.

## Contact Information
For questions or feedback, please reach out to **[sweetykinzu2@gmail.com] | [Kinza Asif]**


**Feel free to customize any sections, especially the contact information and any additional details you want to include!**
