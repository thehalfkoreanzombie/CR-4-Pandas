# My Fourth Code Review: Pandas

## Alex Wallace

## Description
For this project, I had to take a data set called dataset.csv and turn it into a pandas DataFrame. I then had to do a couple of tasks using the DataFrame:

- I changed the 'duration_ms' values from strings to integers
- I converted the amount of milliseconds in the 'duration_ms' columns to minutes
- I renamed the 'duration_ms' column to 'minutes_long'
- I used value_counts to show how many times FKA twigs appears in the 'artists' column
- I used .groupby to get the max danceability rating for each genre (114 total)
- I used shape to count the amount of rows and columns, then dropped the 'valence', 'tempo', and 'time_signature' columns. I then used shape to prove that three columns disappeared
 
## Setup/Installation Requirements
In order to set this up, you will need to make a directory for your file and then switch over to that directory. Then, create a virtual environment for python 3 to work in. Change into your virtual environment using source venv/bin/activate. You will need to install the requirements.txt file (pip install -r requirements.txt). This will allow you to use jupyterlab and pandas. Download the dataset required for the code by using the link https://www.kaggle.com/datasets/maharshipandya/-spotify-tracks-dataset/data. 

## Known Bugs
I used a try/except to make sure no errors were created in the ms_to_minutes function, just in case the values are already integers. Might not be necessary, but I did it just in case.

I renamed the column before applying the map to prevent a column name error

## License
Copyright 2023 Alex Wallace

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
