import pandas as pd
import matplotlib.pyplot as plt

%matplotlib inline

school = pd.read_csv("/Users/charleslai/Documents/2019/Makathon/Python/Makathon Project/SAT__College_Board__2010_School_Level_Results.csv")
students = school[['School Name', 'Critical Reading Mean', 'Mathematics Mean', 'Writing Mean']]
students_data = students.head(12)
students_data_na = students_data.dropna()
students_data_list = students_data_na.sort_values('Mathematics Mean', ascending=True)
school_data_group = students_data_list.set_index('School Name')
school_data_plot = school_data_group.plot(kind='barh', title="New York City School Level College Board SAT Results 2010",figsize=(15,13))
school_data_plot.set_xlabel("SAT MEAN SCORES")
school_data_plot.set_ylabel("NYC HIGH SCHOOLS")
school_data_plot.grid(which='major', linestyle='-', linewidth='0.5', color='grey')
