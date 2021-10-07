# Election_Analysis
Code Version 1.0

## Project Overview
A colorado Board of Elections employee has given you the following task to complete the election audit of a recent local congressional election, give also a resolution process by candidate and county winners.

## Election Audit Results 
the following election outcomes was gived from the analysis, helped by commnets in the coding to assure the code is documented for other developers: 

### How many votes were cast in this congressional election?
369,711 voted for the election.

### Provide a breakdown of the number of votes and the percentage of total votes for each county in the precinct.
County Votes:
Jefferson: 10.5% (38,855)

Denver: 82.8% (306,055)

Arapahoe: 6.7% (24,801)

### Which county had the largest number of votes?
Denver had the largest number of votes

### Provide a breakdown of the number of votes and the percentage of the total votes each candidate received.

Charles Casper Stockham: 23.0% (85,213)

Diana DeGette: 73.8% (272,892)

Raymon Anthony Doane: 3.1% (11,606)

### Which candidate won the election, what was their vote count, and what was their percentage of the total votes?

Winner: Diana DeGette
Winning Vote Count: 272,892
Winning Percentage: 73.8%

## Resources 
-Data Source: election_results-csv
-Software Python 3.8 Visual Studio Code, 1.38.1

## Election-Audit Summary
The analysis of the election show that: 
-there were 369,711 votes cast in the election.
-The candidates were: 
    -Charles Casper Stockham
    -Diana DeGette
    -Raymon Anthony Doane
-The candidate results were:
  -harles Casper Stockham recieved 23.0% of the vote and 85,213 number of votes.
  -Diana DeGette recieved 73.8% of the vote and 272,892 number of votes.
  -Raymon Anthony Doane recieved 3.1% of the vote and 11,606 number of votes.
-The Winner of the election was:
  -Candidate (Diana DeGette, who recieved 73.8% of the vote and 272,892 number of votes
  
  ###   Examples to use script for other elections 
   the following code provide standard structre to be used in other elections basen in the modification of data path file (CSV) located in the following location in the code: 
   
   line 9, by modification of path reference
  ```Python script 
  # Add a variable to load a file from a path.
    file_to_load = os.path.join("Resources", "election_results.csv")
  ``` 
  Line 41 to 51 we can perform some modification to get right categorization instead other values to see the information, for this case, Counties and Candidates
  ```Python script 
  
      # For each row in the CSV file.
    for row in reader:

        # Add to the total vote count
        total_votes = total_votes + 1

        # Get the candidate name from each row.
        candidate_name = row[2]

        # 3: Extract the county name from each row.
        county_name = row[1]
   ```
    Finally, feel free to take reference into the code by PyPoll.py file located in the repository "Election Analysis"
    [Rep](https://github.com/JulioAQuintana/Election_Analysis)

