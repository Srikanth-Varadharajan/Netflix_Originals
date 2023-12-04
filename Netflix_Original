<ol>
<li>Importing Libraries:</li><br/>
import pandas as pd: Imports the Pandas library and aliases it as pd.<br/>
import numpy as np: Imports the NumPy library and aliases it as np.<br/>
import matplotlib.pyplot as plt: Imports the Matplotlib library for data visualization and aliases it as plt.<br/>
<li>Loading Data:</li><br/>
#Netflix=pd.read_csv("/kaggle/input/netflix-original-films-imdb-scores/NetflixOriginals.csv"): Reads a CSV file containing data about Netflix original films' IMDb scores and stores it in a Pandas DataFrame named Netflix.<br/>
<li>Exploratory Data Analysis:</li><br/>

<li>print(Netflix.head()): Displays the first few rows of the DataFrame.</li>
print(Netflix.describe()): Provides summary statistics for numerical columns in the DataFrame.<br/>
Quantile Calculation:<br/>
min_IMDB, max_IMDB = Netflix.IMDB.quantile([0.01,1.0]): Calculates the 1st percentile and the maximum IMDb score.<br/>
Filtering Data:<br/>

Netflix1 = Netflix[Netflix.IMDB < min_IMDB]: Filters movies with IMDb scores below the 1st percentile.<br/>
Netflix2 = Netflix[(Netflix.IMDB > min_IMDB) & (Netflix.IMDB < max_IMDB)]: Filters movies with IMDb scores between the 1st percentile and the maximum.<br/>
Data Inspection and Visualization:<br/>

print(Netflix2): Displays information about movies in the filtered range.<br/>
print(Netflix2.isnull().sum()): Prints the count of null values in each column of Netflix2.<br/>
print(Netflix2.shape): Prints the shape (number of rows and columns) of Netflix2.<br/>
plt.hist(Netflix2.Genre, Netflix.IMDB, histtype='bar'): Plots a histogram of IMDb scores based on movie genres.<br/>
Various plt functions set titles, labels, and legend for the plot.<br/>
plt.show(): Displays the histogram.<br/>
</ol>
