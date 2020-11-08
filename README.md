## **OVERVIEW OF THE PROJECT**

This project is about an election audit where information like number of counties, number of candidates, number of voters, votes caste, county with largest number of votes, candidate 
with highest number of votes along with the percentages and the winning candidate is analysed. The analysis has been presented to the election Commission using Python programming language.

## **ELECTION AUDIT RESULTS**

The result of this audit is given below:

**How many votes were cast in this congressional election?**

Total 369711 votes were caste.

**Provide a breakdown of the number of votes and the percentage of total votes for each county in the precinct.**

**County** ,		**Percentage of votes**	,	**Total Votes**

Jefferson  , 	 10.5%		,		        38,855

Denver	   ,     82.8% 		,		        306,055

Arapahoe   ,     6.7% 		,	        	24,801

**Which county had the largest number of votes?**

Denver got the largest number of votes.

**Provide a breakdown of the number of votes and the percentage of the total votes each candidate received.**

**Candidate**	,		**Number of Votes**	,	**Percentage of Votes**

Charles Casper Stockham ,	85,213	,		23.0%

Diana DeGette	,		    272,892	,		73.8%

Raymon Anthony Doane	,	11,606	,		3.1%

**Which candidate won the election, what was their vote count, and what was their percentage of the total votes?**

*Winner:* 		        Diana DeGette

*Winning Vote Count:* 	272,892

*Winning Percentage:*	    73.8%

The output of the Election Analysis has been saved in a text file and below picture is the extract of the text file showing the above information.

<img src="Election Analysis.PNG"><img>

The below part of the code was used to get the Extract of the information above.

'''
## Print the final vote count 
    election_results = (
        f"\nElection Results\n"
        f"-------------------------\n"
        f"Total Votes: {total_votes:,}\n"
        f"-------------------------\n\n"
        f"County Votes:\n")
    print(election_results, end="")
'''
 ##  Print the county with the largest turnout to the terminal
    winning_county_summary = (
        f"-------------------------\n"
        f"Largest County Turnout: {largest_county}\n"
        f"-------------------------\n")
    print(winning_county_summary)
'''
## Print the winning candidate 
    winning_candidate_summary = (
        f"-------------------------\n"
        f"Winner: {winning_candidate}\n"
        f"Winning Vote Count: {winning_count:,}\n"
        f"Winning Percentage: {winning_percentage:.1f}%\n"
        f"-------------------------\n")
    print(winning_candidate_summary)
'''


## **ELECTION AUDIT SUMMARY**

The coding used to analyse this election can be used for the dataset of any election if below modifications are done in the algorithm.

*This code is based on three columns data "Ballot ID, County Name and Candidate Name" in the same sequence. The code used to extract data is using the specific column number but if 
in any other data set, the sequence of these columns is changed then this code will not work. To overcome this problem, we can use different collection of objects than **List**. 
This collection of objects is **Tuple** because Tuple cant be changed like **lists**.

*Another way of tackling the sequence of data problem is to use **Pandas**, it is much more efficient to bring in specific columns from CSV file.  


