# Overview of Election Audit
An audit of an election was requested. An number of deliverables were desired.

# Election Audit Deliverables
- How many votes were cast in this congressional election?
- Provide a breakdown of the number of votes and the percentage of total votes for each county in the precinct.
- Which county had the largest number of votes?
- Provide a breakdown of the number of votes and the percentage of the total votes each candidate received.
- Which candidate won the election, what was their vote count, and what was their percentage of the total votes?

# Data sources for the election audit
A data file, election_results.csv has been supplied to perform the analysis against.

# Election-Audit Results
The approach for this audit was to use python, a flexible programming language, to gather data from a standardized data file. The script would also output the results to the terminal the python script is run from as well as to a text file. A text file is easily readable on current operating systems. It is also very portable in that it can be distributed as need with nothing more than an email.

The terminal and the text file outputs can be seen below in Figure 1 & 2.

![Eelection Audit Outputs](/analysis/Election_Analysis_Pics.png)

The results of the election audit are as follows:
- There were 369,711 votes cast in the election
- The county vote breakdown was as follows:
    - Jefferson county had 10.5% of the votes which totaled 38,855.
    - Denver county had 82.8% of the votes which totaled 306,055.
    - Arapahoe county had 6.7% of the votes which totaled 24,801.
- Denver county had the largest number of votes cast.
- The candidate vote breakdown was as follows:
    - Charles Casper Stockham had 23.0% of the votes which totaled 85,213 votes.
    - Diana DeGette had 73.8% of the votes which totaled 272,892 votes.
    - Raymon Anthony Doane had 3.1% of the votes which totaled 11,606 votes.
- The winner of the election was Diana DeGette with a winning percentage of 73.8% and 272,892 votes.

# Election Audit Summary
As can be seen in Figures 1 & 2 above, this script puts out a very simple and concise analysis of a structured data file. With a few simple modifications, this script can be adapted to work with any election data file as long as it is a comma seperated file (CSV).
- The script can be modified to prompt the user for the file name, file location and the data comlumn header names. The script could then be modified to open the csv data file and actually search for which column the desired election data resides in making the exact structure and location of the data file flexible.
- The script can also be modified, in addition to out-putting a text file, to output an email contaning the text file. All that would be required is the addition of prompts asking the user for their email address and their email servers smptp drop box location.