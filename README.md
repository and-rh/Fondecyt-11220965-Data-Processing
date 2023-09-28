#   Fondecyt 11220965 Data Processing / Using Annex86 Data Analysis Package

## Description:
Using PurpleAir air quality measurement sensors (https://www2.purpleair.com/), continuous measurements of PM 2.5, PM 10, Humidity, and Temperature were obtained from 20 residential houses in the city of Santiago de Chile. The data collection campaign took place between March 25, 2023, and September 14, 2023. The collected data was processed through the Annex86 library (https://iea-ebc-annex86.github.io/annex/).

### Input Files:
The script reads multiple Excel (.xlsx) files with two sheets:
1. The first sheet contains the raw data, including a time_stamp column.
2. The second sheet contains the configuration data.

### Output:
The script provides:
1. Prepared datasets for each Excel file, processed according to their respective configurations.
2. Analysis objects for each dataset containing environmental data measurements.
3. Statistical summaries of the analysis objects.

### How to Run:
1. Place the script and the Excel files in the same directory.
2. Open the script in an R environment or RStudio.
3. Ensure the file paths and names in the script match the actual files.
4. Run the script.

### Data Structure:
The raw data in Excel files should be structured with a time_stamp column and respective environmental measurement columns. The configuration sheet should be compatible with the annex_check_config function from the annex library.

### Limitations:
1. The script reads and processes each file individually; thus, any comparative analysis or merging of datasets needs to be performed additionally.
2. Any inconsistencies in the configuration sheets may lead to errors during the run. Ensure the correctness of the configurations in Excel files.

### Additional Information:
1. Each analysis is done with respect to Etc/GMT-3 timezone. Adjust the timezone according to your needs if required.
2. Ensure that the Excel files are structured properly, with the correct sheet names and column names to avoid any errors during the run.

