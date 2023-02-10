# Code Review: Spark

#### By Drew White

#### Code Review - Demonstrating the use of Apache Spark

## Technologies Used


* Python
* Apache Spark
* Pandas
* Matplotlib
* Google BigQuery

</br>

## Description:
### Set Up the Data
- [x] Read `coffee.csv` file into a Spark DataFrame.
- [x] All the columns are floats except for the 'Date' and 'Currency' columns.

### Columns from Aggregate Functions
- [x] Add column `daily_diff` to the DataFrame where the values are the difference between 'Open' and 'Close'.

- [x] Add column `high_low` to the DataFrame where the values are the difference between 'High' and 'Low'.

- [x] Add column`volume_100` to the DataFrame where the values are 'True' if the volume for that day was 100 or above, and otherwise 'False'.

- [x] Add column `abs_diff` that contains the absolute values of the numbers in that column.

- [x] Compute a column `net_sales` which is the average of opening, high, low, and closing cost times the volume.

### Stats
- [x] Find the average of the values in the column that has the absolute values of the difference between 'Open' and 'Close'.

- [x] Get the count of values where the 'Volume' was less than 100.

- [x] Find the average 'Open' value.

- [x] Get the highest 'High' value.

### Write File
- [x] Save your DataFrame (including the four added columns) to /data as a parquet file. Exclude the /data directory from Git.


_Net Sales:_  
<img src="./images/net_sales.png"> 

## Bonus

:star: Use Matplotlib to create a visualization (i.e. a chart) using the coffee data.


:star: Include code in the pipeline to write the Parquet file to BigQuery.

<br>

## Setup/Installation Requirements

* Clone by inputting following into terminal: 
  ```bash
  git clone https://github.com/Drewrwhite/data_week_13.git
  ```
* Navigate to directory:
  ```bash
  cd <directory>
  ```
* Create a virtual environment:
  ```bash
  python3.7 -m venv venv
  ```
* Activate virtual environment:
  ```bash
  source venv/bin/activate
  ```
* Install requirements:
  ```bash
  pip install -r requirements.txt
  ```
* Open directory in VSCode:
  ```bash
  code .
  ```
* Navigate to `data`:
  ```bash
  cd data
  ```
* Run get_data.sh:
  ```bash
  ./get_data.sh
  ```

</br>

## Known Bugs

* No known bugs

<br>

## License

[MIT](./license.txt)

_If you find any issues, please reach out at: **d.white0002@gmail.com**._

Copyright (c) _2023_ _Drew White_

</br>
