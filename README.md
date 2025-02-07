# CSV Scourgify Script

## Description
This Python script reads a CSV file containing names formatted as "Last, First" and converts it into a cleaner format with separate "first" and "last" columns. The processed data is then written to a new CSV file.

## Requirements
- Python 3
- `sys` module (built-in)
- `csv` module (built-in)

## Usage
Run the script from the command line with:
python script.py input.csv output.csv


### Command-Line Arguments
- `input.csv`: The source CSV file with columns `name` and `house`.
- `output.csv`: The destination file where cleaned data will be saved.

## Functionality
1. **Argument Validation**
   - Ensures exactly two command-line arguments (input and output files) are provided.
   - Checks that the input file has a `.csv` extension.

2. **File Handling**
   - Reads from `input.csv`.
   - Writes cleaned data to `output.csv`.

3. **Data Transformation**
   - Splits the `name` column into `first` and `last`.
   - Writes data with new headers: `first`, `last`, and `house`.

## Error Handling
- Exits with an error message if the wrong number of arguments are provided.
- Exits if the input file is not a CSV.
- Exits if the input file is not found.

## Example
**Input (`input.csv`):**
```csv
name,house
Potter, Harry,Gryffindor
Malfoy, Draco,Slytherin
```

**Output (`output.csv`):**
```csv
first,last,house
Harry,Potter,Gryffindor
Draco,Malfoy,Slytherin
```

