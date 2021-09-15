# Exploratory Data Analysis Sports
This is one of the  internship tasks given by The Sparks Foundation i.e GRIP(Graduate Rotational Internship Program ). Here, I Performed ‘Exploratory Data Analysis’ on dataset ‘Indian Premier League’.
As a sports analysts, find out the most successful teams, players and factors contributing win or loss of a team. Suggest teams or players a company should endorse for its products. StoryBoards - explaining the charts and interpretations. Use annotations, animation and images.

## Objectives
•	To find the team that won the most number of matches in a season.

•	To find the team that lost the most number of matches in a season.

•	Does winning toss increases the chances of victory.

•	To find the player with the most player of the match awards.

•	To find the city that hosted the maximum number of IPL matches.

•	To find the most winning team for each season.

•	To find the on-field umpire with the maximum number of IPL matches.

•	To find the biggest victories in IPL while defending a total and while chasing a total.


## Data Preparation and Cleaning
The dataset consist of data about IPL matches played from the year 2008 to 2019. IPL is a professional Twenty20 cricket league founded by the Board of Control for Cricket in India (BCCI) in 2008. The league has 8 teams representing 8 different Indian cities or states. It enjoys tremendous popularity and the brand value of the IPL in 2019 was estimated to be ₹475 billion (US$6.7 billion). So let’s analyze IPL through stats. There are 756 rows and 18 columns. 756 rows imply that there were 756 IPL matches held between 2008 and 2019.

The dataset has 18 columns. Let’s get acquainted with the columns.
•	id: The IPL match id.

•	season: The IPL season

•	city: The city where the IPL match was held.

•	date: The date on which the match was held.

•	team1: One of the teams of the IPL match

•	team2: The other team of the IPL match

•	toss_winner: The team that won the toss

•	toss_decision: The decision taken by the team that won the toss to ‘bat’ or ‘field’

•	result: The result(‘normal’, ‘tie’, ‘no result’) of the match.

•	dl_applied: (1 or 0)indicates whether the Duckworth-Lewis rule was applied or not.

•	winner: The winner of the match.

•	win_by_runs: Provides the runs by which the team batting first won

•	win_by_runs: Provides the number of wickets by which the team batting second won.

•	player_of_match: The outstanding player of the match.

•	venue: The venue where the match was hosted.

•	umpire1: One of the two on-field umpires who officiate the match.

•	umpire2: One of the two on-field umpires who officiate the match.

•	umpire3: The off-field umpire who officiates the match



The following inferences can be made from the describe() method:

•	The .csv file has data of IPL matches starting from the season 2008 to 2019.

•	The biggest margin of victory for the team batting first(win_by_runs) is 146 runs.

•	The biggest victory of the team batting second(win_by_wickets) is by 10 wickets.

•	75% of the victorious teams that bat first won by a margin of 19 runs.

•	75% of the victorious teams that bat second won by a margin of 6 wickets.

•	There were 756 IPL matches hosted from 2008 to 2019.


It’s imperative to know the count of NaN values for each column before we proceed further.
The column ‘umpire3’ has a significant number of NaN values. As the off-field umpire parameter is insignificant, we can drop this column. The other columns that have Nan values are of type object(Pandas equivalent of Python String data type) and are very few in number(<=7).


## EDA
### Number of matches played in each of the IPL season

![image](https://user-images.githubusercontent.com/70087327/133458319-847853bd-ca34-42d7-9422-299763f42b0d.png)

•	In 2013 maximum of 76 matches are played followed by 2012, 2011.
•	Usually, number of matches ranges to 60.

### Top 10 Man of the Match

![image](https://user-images.githubusercontent.com/70087327/133458588-2cf21125-dd97-42e5-bf14-b067083e05b3.png)

•	Chris Gayle is leading the pack followed by AB de Villiers

### Number of Matches won by Each IPL Team

![image](https://user-images.githubusercontent.com/70087327/133458835-85f4f737-804e-4c4d-9fcb-05f1ed7919ec.png)

• Mumbai Indians are the winners of most matches followed by Chennai super kings

### Total matches Vs Matches Won & Percentage of Matches Won
![image](https://user-images.githubusercontent.com/70087327/133459329-9f206e04-3aad-47fd-9f0d-ae8413328c99.png)

• Out of total matches played Delhi capitals has highest winning percentage , though Mumbai Indians has played most matches and won most matches.

### Most hosted Venues

![image](https://user-images.githubusercontent.com/70087327/133459713-48ac9d2b-962c-470f-8cb4-c4a67e0594ee.png)

• Eden Gardens are the most frequently hosted stadium.

### Toss Decision

![image](https://user-images.githubusercontent.com/70087327/133461926-7ae7557f-b005-4f1a-bea0-c830a21d1830.png)

• Mostly when a team wins the toss, the chances of choosing fielding is higher than the batting.

• we will check what will be the chances of winning after winning the Toss



### Toss Winning VS Winning Chances

![image](https://user-images.githubusercontent.com/70087327/133462109-eeaddbc4-f895-453b-af50-5d4cd91d3e64.png)

•	Mumbai Indians has won most of the times but their chance of winning match after winning toss is 57.1% only.

## Runs Analysis

### Delivery Metrics

![image](https://user-images.githubusercontent.com/70087327/133462499-3b7aac17-de53-4c5d-bde5-674a5837fd73.png)


### Dismissal types

![image](https://user-images.githubusercontent.com/70087327/133462759-d4150799-3d71-4338-9895-a09ecd0ec221.png)


• Most type of Dissmisal is Caught and bowled

### Total Runs in Seasons

![image](https://user-images.githubusercontent.com/70087327/133462909-b6779c39-4e5c-4aa4-8b26-9df1a66b669f.png)


• In 2013 the number of total runs is more compared to 2012,2011 or the other years , as there were more number of matches were conducted than usual.

### Average Runs per match Across the Seasons

![image](https://user-images.githubusercontent.com/70087327/133463099-471ebda5-0f71-42c0-b442-f602d2c129f9.png)


• In 2018 the average run per match are very high than usual.

### Run Rate

![image](https://user-images.githubusercontent.com/70087327/133463315-60f68322-e134-49c5-90a5-9e5459099718.png)

• The Run rate at the starting over like 2nd and 3rd over is usually higher and goes on decresing trend till 20 overs

### Top Wicket Taker

![image](https://user-images.githubusercontent.com/70087327/133463494-8c7acfa8-1f70-4403-b02c-34ea5d6cb373.png)

• SL Malinga is the highest wicket taker from 2008 to 2018 with 170 wickets

### Purple Cap holder for year 2017

![image](https://user-images.githubusercontent.com/70087327/133463640-d257307a-6baa-448f-98fe-5883791e4da9.png)


• In 2017, B Kumar won the purple cap.

### Most Runs by batsmans

![image](https://user-images.githubusercontent.com/70087327/133463842-50b1bf02-4718-4b5c-9afc-e157cde4d6e7.png)


• V Kohli has scored top score followed by SK Raina and RG sharma

### Orange Cap holder for year 2017

![image](https://user-images.githubusercontent.com/70087327/133464075-cc5a62af-44b0-4ba6-85d1-5f174d215165.png)


• In 2017 , the Orange cap winner is DA Warner.

### BATSMAN-METRICS

![image](https://user-images.githubusercontent.com/70087327/133464244-3c7bbcee-6311-423f-a64b-b4c088fd75a2.png)

### Most Sixes by batsman in IPL

![image](https://user-images.githubusercontent.com/70087327/133464338-5c226de4-fd7a-470a-ad00-c48007a0112c.png)

• S Dhawan is leading the pack by a considerable margin.

### Most Fours by batsman in IPL

![image](https://user-images.githubusercontent.com/70087327/133464513-2e12d5c2-2fec-4fd3-a00d-7ad9d9bf3a5d.png)


• CH Gayle has highest number of 4's scored in all the IPL Matches.


### Most Run-out faced by any batsman in IPL

![image](https://user-images.githubusercontent.com/70087327/133464712-7ef353c3-6f65-4838-8d91-3dded9edbc4b.png)

• G Gambhir has faced most of his out by Run-out followed by S Dhawan.


### Top Wicket takers in IPL

![image](https://user-images.githubusercontent.com/70087327/133465032-5fa0bf21-4436-4f60-b990-283a170cbaa7.png)


• SL Malinga has taken 170 wickets all togther from 2008-2019 IPL matches


### Most Catches across IPL

![image](https://user-images.githubusercontent.com/70087327/133465160-29bfa92d-8f39-455f-a714-f09bb412749b.png)


• KD Karthik has taken most of wickets by 109 catches followed by SK Raina

### Most RunOuts by fielder across IPL

![image](https://user-images.githubusercontent.com/70087327/133465300-b9fa1de6-af38-45d7-9c1a-a61fd68f6c57.png)


• MS Dhoni has tacken 23 wickets by run-out the batsman



## Conclusions

•	Mumbai Indians is the most successful team in IPL.

•	Mumbai Indians has won the most number of toss.

•	There were more matches won by chasing the total(419 matches) than defending(350 matches).

•	When defending a total, the biggest victory was by 146 runs(Mumbai Indians defeated Delhi Daredevils by 146 runs on 06 May 2017 at Feroz Shah Kotla stadium, Delhi).

•	When chasing a target, the biggest victory was by 10 wickets(without losing any wickets) and there were 11 such instances.

•	The Mumbai city has hosted the most number of IPL matches.

•	Chris Gayle has won the maximum number of player of the match title.

•	Winning toss gives a slight edge(52% probability of winning) against the opponents.


•	Five Indian players have figured in the top ten IPL players list.

•	S. Ravi(Sundaram Ravi) has officiated the most number of IPL matches on-field.

•	Eden Gardens has hosted the maximum number of IPL matches.

•	Till 2019, 40 venues have hosted 756 IPL matches.

