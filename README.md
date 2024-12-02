# TASK-1----Data-Preparation

#Import required packages
import pandas as pd
import plotly.express as px
import dash
from dash import dcc
from dash import html

#Read the airline data into pandas dataframe
airline_data =  pd.read_csv('https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-DV0101EN-SkillsNetwork/Data%20Files/airline_data.csv', 
                            encoding = "ISO-8859-1",
                            dtype={'Div1Airport': str, 'Div1TailNum': str, 
                                   'Div2Airport': str, 'Div2TailNum': str})

#Randomly sample 500 data points. Setting the random state to be 42 so that we get same result.
data = airline_data.sample(n=500, random_state=42)

#Pie Chart Creation
fig = px.pie(data, values='Flights', names='DistanceGroup', title='Distance group proportion by flights')


![image](https://github.com/user-attachments/assets/04c02107-398d-4433-a2b9-8fe41b216d7d)

# i did install the following:
![image](https://github.com/user-attachments/assets/80f11d37-6cd1-4be1-8549-9826ca735243)

# then i follow the instructions from the forum and still have the same problem
![image](https://github.com/user-attachments/assets/880fa7de-d366-4ad3-b03c-2b63b232f0fd)
![image](https://github.com/user-attachments/assets/652d8e9c-1ea5-4390-ae7c-4208d2613bf1)
