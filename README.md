# SC5002 Lab 2

This lab uses the automobile data set obtained [here](https://archive.ics.uci.edu/dataset/10/automobile).

## Steps
1.  Setting up virtual environment
A `requirements.txt` file was generated from the virtual environment.

2. Dataset loading
The dataset was loaded using `pd.read_csv` and using the link as a argument.

3. Imputation for missing data
Two approaches were used for dealing with missing data. For numerical data, the median was used to simply fill the missing data. For categorical data, the mode was used to fill the missing data. The variables/columns with data was found using dataframe indexing.

4. Encoding categorical data
To handle the nominal data (which has no order), one-hot encoding was used. To handle the ordinal data, label encoding was done to label a unique integer to each cataegory in specific columns.

5. Split into training/test
As per regular ML practice, the training and test set was split with a 20% test ratio.

6. 
