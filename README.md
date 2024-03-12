
## Usage

# Analysis of the Indian Startup Ecosystem
 
This data analysis project is to answer questions that investors have been asking over the years whether investing in an indian startup is the nex venture for them

## Getting Started
Using the CRISP-DM framework for this data analysis project
### Installation

- Use the package manager [pip] (https://pypi.org/project/MySQL-python/)  to install MySQLdb.
- Use the package manager [pip] (https://pypi.org/search/?q=sqlalchemy) to install sqlalchemy.
- Use the package manager [pip] (https://pypi.org/search/?q=pyodbc+&o=) to install pyodbc.  
- Use the package manager [pip] (https://pypi.org/search/?q=scipy&o=) to install scipy.
- Use the package manager [pip] (https://pypi.org/search/?q=python-dotenv&o=) to install dotenv.
- Use the package manager [pip] (https://pypi.org/search/?q=pandas&o=) to install pandas.
- Use the package manager [pip] (https://pypi.org/search/?q=seaborn&o=) to install seaborn.

#### Currency Converter function

'''def curr_converter(df,rate):
    amount_new=[]
    for a in df:
        if a.startswith('$'):
            
            amount_new.append(a.split('$')[1].replace(',',''))
        elif a.startswith('₹'): 
            
            amount_new.append(float((a.split('₹')[1]).replace(',',''))/rate )  
        else :
            amount_new.append(a)    
    return amount_new ```

#### Some methods used in cleaning the data
```data_2021['new'] =  data_2021['Investor'].fillna('inv') +data_2021['Amount'].astype(str) + data_2021['Stage'].fillna('ab') ```

### Categorising the Sectors into 9 groups for easier classification
```
- Technology & Software: Startups primarily focused on developing software, AI, IT solutions, and technology-related services.
- E-commerce & Retail: Startups involved in online retail, e-commerce platforms, marketplace solutions, and retail-focused businesses.
- Finance & FinTech: Startups operating in financial services, banking, financial technology (FinTech), cryptocurrency, and related areas.
- Healthcare & HealthTech: Startups in the healthcare industry, including health technology (HealthTech), telemedicine, medical devices, and healthcare services.
- Education: Startups in the Education industry, including learning,spacetech,data story telling and edtech.
- Energy: Startups in the Energy industry, including Renewable energy,battery technology, EV systems, crude oil and other energy related services.
- Agriculture: Startups in the Agriclture industry, including farming and fishing.
- Hospitality: Startups in the Hospitality industry, including real estate,hotels,homes and hospitality services.
- Others: Startups that do not fit directly into the above categories or have unique business models.
```
#### Using the Willis Kruskal test to test the hypothesis
```
stat, p = kruskal(fintech.Amount, commerce.Amount, health.Amount,tech.Amount,edu.Amount,agric.Amount,energy.Amount,other.Amount)
print('Statistics=%.3f, p=%.10f' % (stat, p))

if p > 0.05:
 print('All sample distributions are the same (fail to reject H0)')
else:
 print('One or more sample distributions are not equal distributions (reject null Hypothesis)')
 ```
## Acknowledgements

 - [Awesome Readme Templates](https://awesomeopensource.com/project/elangosundar/awesome-README-templates)
 - [Awesome README](https://github.com/matiassingers/awesome-readme)
 - [How to write a Good readme](https://bulldogjob.com/news/449-how-to-write-a-good-readme-for-your-github-project)


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
