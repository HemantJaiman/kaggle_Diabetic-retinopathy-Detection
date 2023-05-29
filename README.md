# Challenge from Woven by Toyota

This README file provide information about the code, its functionality, usage instructions, and additional details.

## Table of Contents
1. Description
2. Requirements
3. Installation
4. Run The Code
5. Tests
6. Algorithmic Complexity
7. Directory structure

## Description

This code is designed to find the top X values from a given dataset and retrieve their associated IDs. It can be used to identify the records with the highest values in a dataset.

## Requirements
- Python 3.x
- Required Python packages: heapq, sys, collections, argparse




## Installation

Download the zip to local machine and Unzip the file.
Python 3.x should be installed on the system.
Install the required Python packages by running the following command in the terminal
```
pip install heapq

``` 
Python file can be executed now



## Run The Code
### Execute the following command in the terminal, providing the necessary arguments:

```bash
    python solution.py -f <file_path> -x <top_values>

```
- <file_path>: (Optional) Absolute or relative path to the file containing the records in the specified format. If not provided, the program will read from stdin.
- <top_values>: (Optional) Number of top values to consider. Default value is 3.

### input format
    The program accepts input in the following format:
```bash
    <unique record identifier> <numeric value>
```
Example:

    1426828011 9
    1426828028 350
    1426828037 25
    1426828056 231
    1426828058 109
    1426828066 111

- The input can be provided through a file or through stdin.

### Output Format
The program outputs a list of the unique record identifiers associated with the X-largest values, where X is the specified number of top values.

Example Output:

```bash
    ["1426828028","1426828066","1426828056"]
```
## Tests
The tests.py file contains test cases to validate the functionality and robustness of the code. The tests cover various scenarios, including input from a file, input from stdin, different values of X, and different file sizes.
To run the tests, execute the following command:
```bash
    python tests.py
```

## Algorithmic Complexity

This code has the following algorithmic complexities:

Time Complexity: O(N log X)

N is the number of records in the dataset.
X is the desired number of top values to retrieve.
The code iterates through the dataset once, performing heap operations that take logarithmic time.
Memory Complexity: O(X)

The code uses a min-heap of size X to store the top X values.



## Directory structure:
```
Hemant.jaiman/
├── solution.py
├── README.md
├── tests.py
└── data/
    ├── test_case.txt
```

1. A `solution.py` file in root folder

    Action: 
    
    Run 
    ```bash
    python solution.py -f <file_path> -x <top_values>
    ```

    Results: 
    
    - outputs a list


2. A `data` sub-folder:

    This directory includes test case file-> test_case.txt



3. A `tests.py` file in root folder:

     Action: 
    
    Run 
    ```bash
    python tests.py
    ```

    Results: 
    
    - Execute test cases 
