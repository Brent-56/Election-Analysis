Election-Analysis
Python 3..9.12

### Overview
The purpose of this Analysis was to help with a local congressional election audit. We were tasked with calculating the total number of votes. Then we were tasked with calculating how many votes specific candicates recieved. From there we could determine what percentage of the votes each candidate recieved. This allowed us to determine which candidate won the election.

### Resources
python version 3.9.12
VS Code 1.71.2
election_results.csv
election_results.txt

### Election - Audit Results
There were a total of 369,711 votes casted in this election.
The if statement that determined the winning county and its vote count was 
       
       if (c_votes > winning_county_count) and (c_vote_percentage > winning_c_percentage):
            winning_county_count = c_votes
            winning_county = county_name
            winning_c_percentage = c_vote_percentage
            
We determined it was Devner. After finding out which county it was I printed it with 
       
    winning_county_summary = (
        f"-------------------------\n"
        f"Largest County Turnout: {winning_county}\n"
        #f"Largest Vote Count: {winning_county_count:,}\n"
        #f"Largest Percentage: {winning_c_percentage:.1f}%\n"
        f"-------------------------\n")
    print(winning_county_summary) 
   
   This code displayed the Largest County Turnout as the winning_county which was Denver. 

Denver had 82.8% or (306,055) of the votes.
Jefferson had 10.5% or (38,855) of the votes.
Arapahoe had 6.7% or (24,801) of the votes.

The candidates who ran were Charles Casper Stockham, Diane Degette, and Raymon Anthony Doane.

Charles Casper Stockham had 23.0% or (85,213) of the votes.
Diane DeGette had 73.8% or (272,892) of the votes.
Raymon Anthony Doane had 3.1% or (11,606) of the votes.
Diane Degette won the election with 73.8% or (272,892) of the votes.

### Election - Audit Summary
The Script was good in terms of being able extract information from a CSV file and import it into a txt file with the data organized to the point that is understandable by the masses. This script gives a solid description of votes per county and votes per candidate. In my opinion I think this script is a great to start for any smaller election. It displays all the details we need for a basic analysis such as voter turnout, the winnner, and percentages.

However for a bigger election more detail may be required which means we will need to make modifications to the code. For example instead of just listing voter turnout per county a larger audit may require us to make connections between the county's and the candidates. We may need to implement code that displays what percentage of a specific county voted for a specific candidate. Another example would be we may need to implement code that states each candidates political party and how each county votes in terms of political party preferences. This is a great starter script but more code will be required for bigger projects.


