# Analysis of the Indian Startup Ecosystem
https://img.shields.io/badge/data_analysis-hypothesis_testing
 
This data analysis project is to answer questions that investors have been asking over the years whether investing in an indian startup is the next big venture for them

## Getting Started
This data analysis project is to answer questions that investors have been asking over the years whether investing in an indian startup is the next big venture for them.
Using the CRISP-DM framework for this data analysis project

### Installation and Setup

#### Python Packages Used

- Data Manipulation : ```pandas``` 
- Data Visualization : ```seaborn```
- SQL Database Connection : ```sqlalchemy,pyodbc,python-dotenv```
- Hypothesis Testing: ```scipy```
- Use the package manager [pip] 

### Data
There are four (4) datasets used for analysis which share similiar columns such as company name,founded,headquarter city and other columns. 

#### Source Data
- 2021 startup funding dataset from an SQL database
- 2020 startup funding dataset from an SQL database
- 2019 startup funding dataset from a CSV file
- 2018 startup funding dataset from a CSV file

#### Data Preprocessing
- Include the investment year to each data set.
- Check headers and maintain the same column headers for all datasets
- Get the Dollar/Rupee rate for each year
- Convert all amounts to a common currency,Dollar
- Concatenate the datasets to put them together
- Perform Hypothesis Testing and Exploratory Data Analysis

### Results and Evaluation

- The industry sector fundings are not normally distributed therefore Willis Kruskal test used
- Cleaned Data has 2879 rows with 9 funding sectors and 9 industry sectors.

### Future Work
There is a need to review the data cleaning proprocessing to be able to correctly fish out data entry mix up to make the data cleaner.
 
## Contributions
Contributions, issues, and feature requests are welcome!
Give a ⭐️ if you like this project!

## License
[MIT](https://choosealicense.com/licenses/mit/)

## Conclusion
From my analysis,it is realised that :
- Many startups located in the Bangalore have the highest average investments as compared to other cities therefore it will be easier to find viable startups to invest in that city.
- There is a high average investment needed for the E-Commerce & Retail Sector Sector, an investor is adviced to ventor into other sectors such as Energy,Hospitality,Agriculture and Technology & Software.
- Though many startups looked for other sources of funding such as Debt financing, there are still many other startups in the Seed financing category that investors can invest into. 

## Author

**Emmanuel Chrappah**

- [Profile](https://github.com/rohit19060 "Emmanuel Chrappah")
- [Email](mailto:chrappahkwasi@gmail.com?subject=Hi "Hi!")
