# Election_Analysis

## Overview of the Election Audit
This election audit was set out to accurately tabulate and present results of a multi-county election from the data stored in a .csv file.

## Election Audit Results
- There were 369,711 votes cast in this election
### County Results
- Jefferson county cast 38,855 votes for 10.5% of the total vote. 
- Denver county cast 306,055 votes for 82.8% of the total vote. 
- Arapahoe county cast 24,801 votes for 6.7%% of the total vote. 
- Denver County had a much larger sway in the election with by far the most votes.
### Candidate Results
- Charles Casper Stockham recieved 85,213 votes for 23.0% of the total vote.
- Diana DeGette recieved 272,892 votes for 73.8% of the total vote.
- Raymon Anthony Doane recieved 11,606 votes for 3.1% of the total vote.
- Diana DeGette was the winner of the election with 272,892 votes for 73.8% of the total vote.

## Election Audit Summary
This script could be used to tabulate and present the results of a variety of elections given that the .csv being imported has the same format with the county name in the "1"(2nd) column and the candidate for whom the vote was cast in the "2"(3rd) column. These are the lines concerned : 
  `candidate_name = row[2]` `county_name = row[1]`
If you were importing data in a differently formatted .csv you would have to change the bracketed numbers to corrospond with the proper indices for the candidates and the counties 
        
The other adjustment would need to the code that is loading the .csv and then deciding where to save the results to

```python
file_to_load = os.path.join("an indirect path here to your.csv")
```

```python
file_to_save = os.path.join("an indirect path here to your.txt")
```
