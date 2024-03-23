# DOCUMENTATION ON RUNNING THE ANALYSIS SUCESSFULLY

## Create datebase using Postgres 
`
CREATE TABLE stock_data (
    datetime TIMESTAMP,
    instrument VARCHAR(255),
    open DECIMAL(10, 2),
    high DECIMAL(10, 2),
    low DECIMAL(10, 2),
    close DECIMAL(10, 2),
    volume BIGINT
);
`

## Create a .env file to take in your DataBase details
### The env file should be in this form
`
DB_USERNAME=your_user
DB_PASSWORD=your_password
HOST=localhost or any other host
PORT=5432 or your_port
DATABASE=your_db_name
TABLE_NAME=your_table_name
PATH_TO_FILE=your_path_to_file_name
`
### NOTE: The env file should be in the same folder the main file is

### Run the main.ipynb file.