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

