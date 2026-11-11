# Gas Mileage Data Exploration

This project is a hands-on learning module for exploring a small dataset with Python. It uses pandas to read and summarize tabular data, and Matplotlib to visualize patterns. Instead of written as .py files, the files are jupyter notebooks to help separate concepts for practice and learning: **run the cells, complete the TODOs, and adjust the analyses as you learn.**

## Dataset

`Data/gas_mpg.csv` contains 16 recorded fuel purchases. This is real-world data that the club President has been tracking. Each row represents one refuel and includes:

| Column            | Description                                        |
| ----------------- | -------------------------------------------------- |
| `Date`            | Date of the refuel                                 |
| `Gas_Station`     | Station where fuel was purchased                   |
| `Price_per_Gal`   | Price per gallon                                   |
| `Total_Price`     | Total amount paid                                  |
| `Total_Gallons`   | Fuel purchased, in gallons                         |
| `Range`           | Recorded vehicle range associated with the refuel  |

The data is small enough to inspect directly while still providing useful examples of dates, categories, and numeric values. It can be used to practice checking data types and missing values, calculating summary statistics and correlations, and exploring how purchase cost, fuel quantity, and range vary.

## Learning Objectives

- Load a CSV file from a project subfolder and inspect its rows and columns.
- Convert date text into datetime values and calculate time between fill-ups.
- Summarize numeric columns with statistics such as mean, minimum, and maximum.
- Explore relationships between numeric variables using correlation.
- Group purchases into time periods to calculate monthly fuel spending.
- Build and customize a bar chart, including value labels, axis spacing, and colors that reflect monthly cost.

## Notebooks

- [`Notebooks/data_exploration.ipynb`](Notebooks/data_exploration.ipynb) — general inspection and summary of the dataset.
- [`Notebooks/analysis_total_cost.ipynb`](Notebooks/analysis_total_cost.ipynb) — explores fuel spending over time and practices grouping and charting.

## Getting started

Open the notebooks in Jupyter or another notebook environment. Run the setup/import cell first, then execute the remaining cells in order. The data file is stored in `Data/`; notebook paths such as `../Data/gas_mpg.csv` are relative to the `Notebooks/` directory.

Remember that there are **installation milestones** provided on the GitHub if you are struggling to run your environment or are missing installations.

The project uses Python with pandas, NumPy, and Matplotlib. If needed, install them in your environment with:

```bash
python -m pip install pandas numpy matplotlib
```


## Python Tips

1. **Python is a case sensitive language**: Be careful about capitalizing names, using underscores and names of variables in general. Typing the wrong variable name is the most common error.

2. Python can only ouput visuals with either a **print() statement or a plt.show() statement** if outputting a plot.
```sh
print(dataframe)
```

```sh
print(f"Printing my entire dataframe: {dataframe}") # printing a message with a variable
```

```sh
plt.show()
```


## Jupyter Notebook Tips

1. **Run Notebook cells in order**: Each cell is its own isolated code and running that cell will only run the code inside. If your current cell is dependent on having created something or changed something in a previous cell, then they need to be run in order. 

2. **Start each file by running the import cell**