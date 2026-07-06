# codevedx
internship 


# PROJECT 1 - Data Analysis with Python

import pandas as pd

data = {
    'Name': ['Arun', 'Priya', 'Rahul', 'Divya', 'Karan'],
    'Math': [78, 85, 67, 90, 72],
    'Science': [80, 88, 70, 92, 75],
    'English': [74, 81, 69, 95, 70]
}

df = pd.DataFrame(data)

print("Student Marks Data")
print(df)

df['Average'] = (df['Math'] + df['Science'] + df['English']) / 3

print("\nAverage Marks")
print(df[['Name', 'Average']])

topper = df.loc[df['Average'].idxmax()]

print("\nTop Scorer")
print(topper)

