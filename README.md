# Covid19_Stats
This is a python script that is used to analyse state wise statistic of Covid 19 in India.
Step 1 : Clone the repository 
Step 2 : Download the latest .csv file of the from 	https://api.covid19india.org/csv/latest/state_wise_daily.csv
Change the path to the place where the file state_wise_daily.csv is stored in your computer in these lines of code :
- read_file = pd.read_csv (r'your_path\state_wise_daily.csv', low_memory=False)
- read_file.to_excel (r'your_path\state_wise_daily.xlsx', index = None, header=True)
- wb = load_workbook(r'your_path\state_wise_daily.xlsx')
- wb.save(r'your_path\state_wise_daily.xlsx')
Step 3 : Run the Coronavirus.py python script 

Result 
39 excel files would be stored in your current working directory , one for each state (includes UT as well)
The excel file would have 9 columns 
1st Column : Date 
2nd Column : Number of Confirmed Cases 
3rd Column : Number of Recovered Cases 
4th Column : Number of Deaths
5th Column : Cumulative Number of Confirmed Cases
6th Column : Cumulative Number of Recovered Cases
7th Column : Cumulative Number of Deaths 
8th Column : Recovery Rate (Cumulative Number of Recovered Cases/Cumulative Number of Confirmed Cases*100)
9th Column : Death Rate (Cumulative Number of Deaths/Cumulative Number of Confirmed Cases*100)
