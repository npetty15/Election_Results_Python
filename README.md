# Election Audit with Python

## Overview of Election Audit

The purpose of this review was to use Python to create a script that would automatically tabulate the total votes and percentage of the total votes for the counties and the candidates from the last election. 

Based on that analysis the largest county and election winner was determined. The results of the audit were saved to a text file and showed several results:

1) Total votes in election
    
2) Votes by county and largest voter turnout by county
    
3) Votes by candidate, which included total votes by candidate and percentage of total votes
    
4) Election winner, with total votes by candidate and percentage of total votes.

![election_results](https://user-images.githubusercontent.com/100856534/162007513-773edbc0-2d0c-4057-bbe6-b7d846b0e865.png)

## Election Audit Analysis 

1) How many votes were cast in this congressional election?

      * $369,711 votes were cast in Arapahoe, Denver, and Jefferson counties.  

When the data was received, it was determined that each row in the csv file was one vote. The code needed at this point was to count each row to get the total votes in the election. 

![total_votes_code](https://user-images.githubusercontent.com/100856534/162019305-299ba3ec-b07b-4db6-b27a-16168e8211c0.png)
      
2) Provide a breakdown of the number of votes and the percentage of total votes for each county in the precinct.
  
      * Arapahoe County: Total votes- $24,801 Percentage of total votes- 6.7%
      * Denver County: Total votes- $272,892 Percentage of total votes- 73.8%
      * Jefferson County: Total votes- $38,855 Percentage of total votes- 10.5%
 
Using the same row function as the total vote count, we can nest an "if-statement" that would tabulate the total county vote and percentage
 
 ![county_votes_percentages](https://user-images.githubusercontent.com/100856534/162021246-ac87401b-9afe-49c8-8a92-714c9daf5995.png)
      
3) Which county had the largest number of votes?
   
      * Denver County had the largest voter turnout
      
In previous code, we were able to determine the total amount of votes per county and thier percentages. Using that data, we can determine which county had the largest voter turnout. 

![largest_voter_turnout](https://user-images.githubusercontent.com/100856534/162022229-7597ed3b-4b96-4351-96ee-514708a64473.png)
      
4) Provide a breakdown of the number of votes and the percentage of the total votes each candidate received.
   
      * Charles Casper Stockham had $85,213 total votes, which was 23% of the vote.
      * Diana DeGette had $272,892 total votes, which was 74% of the total vote.
      * Raymon Anthony Doane had $11,606 total cotes, which was 3% of the total vote.

The code to determine this was roughly the same as it was for the per count votes and total votes percentage. The difference would be the variables that were used, such as candidate_options, candidate_name, etc. 
      
5) Which candidate won the election, what was their vote count, and what was their percentage of the total votes?
  
      * Diana Degette won the election with a total of $272,892 votes. This gave her the majority of the total votes at 74% ballots cast in her name.

The code for this one is similar to the one that was used to determine largest voter turnout county. Again, the main difference here would be the variables used and for this portion the percentage of vote was included in the printed section in the text file. 
 
## Election Audit Summary

The script that was developed for this election audit was based on three counties, Arapahoe, Denver, and Jefferson, and it works well in delivering the information for the audit review. However, I believe that we can translate this script to different elections around the state or county. If provided the information as we were with the original three counties in the same format (e.g. csv). We could make any number of adjustments to allow the script to work. 

As I went through this review, we originally had it complete only one process, and that was providing the vote per candidate, as well as percentage of vote per candidate. Based on that we provided the winner. Then it was further discussed that we wanted to see what the voter turnout would be based on county. As you can see based on the information available to us, using Python can adapt the script to what may be needed in the future.

### Example 1: Votes for Candidates per County ###

One additional item we could add based on the current information that we have is determining what amount of votes each candidate has per county. This might be useful for the election board to see if there is any disparity between candidates by county. Or it might be useful for the candidates themselves to see where they may have lacked voter support.

### Example 2: Votes for a Yes/No Ordinance ###

<<<<<<< HEAD
Another item that could be adapted to this script, is if there was an ordinance that the voter only had two options for. This would basically be a True or False review of the vote. One example here would be if a school district requested additional property taxes levies to help pay for repairs. The voter would go to the polls and vote yes (true) or no (false).
=======
Another item that could be adapted to this script, is if there was an ordinance that the voter only had two options for. This would basically be a True or False review of the vote. One example here would be if a school district requested additional property taxes levies to help pay for repairs. The voter would go to the polls and vote yes (true) or no (false). 
   
>>>>>>> 9beef16be631153a86a6333f6af957abd11c44e1
