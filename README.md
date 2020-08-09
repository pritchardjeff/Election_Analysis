# Election_Analysis

## Overview of Project

Originally, we were asked to write a script that would quickly and accurately determine the winner of an election based on data provided in a CSV file.

After writing a script to determine the winner of an election, we were asked by the election commission to pull a few additional data points from the election data.

The additional items included voter turnout for each county, the % of votes from each county out of the total count, and the county with the highest turnout.

The script is the file below:

[PyPoll_Challenge.py] (https://github.com/pritchardjeff/Election_Analysis/blob/master/PyPoll_Challenge.py)

### Election-Audit Results

- Total Votes Cast  - 369,711
- Number of votes and the percentage of total votes for each county:
  - Jefferson: 10.5% (38,855 Votes)
  - Denver: 82.8% (306,055 Votes)
  - Araphahoe: 6.7% (24,801 Votes)
- County with largest number of votes was Devner
- Breakdown of the number of votes and the percentage of the total votes each candidate received 
  - Charles Casper Stockham: 23.0% (85,213 Votes)
  - Diana DeGette: 73.8% (273,892 Votes)
  - Raymon Anthony Doane: 3.1% (11,606 Votes)  
- Winning Candidate was Diana DeGette: 73.8% (273,892 Votes)

The result output can be found in the following file:

[election_analysis.txt] (https://github.com/pritchardjeff/Election_Analysis/blob/master/Analysis/election_analysis.txt)

### Election-Audit Summary

#### Proposal on how the script can be used for other elections

The script used in the congressional election can be used in other elections as long as there is an already clean CSV file with the following fields in the following order:

- Ballot ID - Unique ID associated with each vote
- County - Geographic region the vote occurred 
- Candidate - The party/person being elected

If a new data source is used with data in an order different than the one listed above, then the following modifications must take place:

1. The Candidate must be changed to the column of the CSV where it is located. Currently set to look for the Candidate in row 2 (Column C of the CSV).
2. The County must be changed to the column of the CSV where it is located. Currently the code is set to look for the county/geographic region in row 1 (Column B of the CSV).

See image below for where to change the code mentioned above:

![Election_Analysis_Row_Selection]. (https://github.com/pritchardjeff/Election_Analysis/blob/master/Election_Analysis_Row_Selection.png)





