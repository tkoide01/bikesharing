# Bike-sharing Program Analysis

## Overview of the Analysis
Analyzing data from Citibike bike-sharing program in New York City area, provide the visualization of bike trip data to convince investors about launching a bike-sharing program in Des Moines. In order to do so, we will make following visualizations:  

1. Show the length of time that bikes are checked out for all riders and genders
2. Show the number of bike trips for all riders and genders for each hour of each day of the week
3. Show the number of bike trips for each type of user and gender for each day of the week.

Lastly, we combine these visualizations into Tableau dashboards and stories as final presentations for investors.
## Resources
- Data Source: 201908-citibike-tripdata.csv from the website *Citi Bike System Data* URL: <https://www.citibikenyc.com/system-data>
- Software: Jupytor Notebook, Tableau Public

## Election-Audit Results
The Analysis of the election show that:
- There were 369,711 votes cast in the election.
- The candidates were:
  - Charles Casper Stockham
  - Diana DeGette
  - Raymon Anthony Doane
- The candidate results were:
  - Charles Casper Stockham received 23.0% of the vote and 85,213 number of votes.
  - Diana DeGette received 73.8% of the vote and 272,892 number of votes.
  - Raymon Anthony Doane received 3.1% of the vote and 11,606 number of votes.
- The winner of the election was:
  - Diana DeGette, who received 73.8% of the vote and 272,892 number of votes.
Below is the screen shot of "election_results.txt" showing the result of analysis from the written code.

![](Resources/Election_analysis_terminal.png)

## Election-Audit Summary
Lastly, I would like to propose that the written Pythone code for this project is applicable for any election.

For example, if we want to run the same analysis with different data source, we can modify the script as follow to allow the code pull the data source.
```
# Add a variable to load a file from a path.
file_to_load = os.path.join( "Resources", "election_results_modified.csv")
# Add a variable to save the file to a path.
file_to_save = os.path.join("analysis", "election_analysis_modified.txt")
```
Also, if we see learn that modified data source in this case has different numbers of columns as shown below, we can modify the below script to accomodate as well.

![](Resources/Election_analysis_terminal_4.png)

```
  # Get the candidate name from each row.
  candidate_name = row[3]

  # Extract the county name from each row.
  county_name = row[2]
```
So as long as we ensure that code refers to appropriate columns for items, this Election-Audit code can run the analysis to output the winning candidate, his/her vote count, and the percentage of vote to the total vote count.
