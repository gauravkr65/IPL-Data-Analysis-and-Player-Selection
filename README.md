# IPL-Data-Analysis-and-Player-Selection
This project analyzes historical IPL data to identify top-performing players in batting and bowling. Using statistical techniques, it recommends player selection and team composition strategies for a successful IPL team. The project also includes regression analysis to predict player performance and offers data visualizations for insights. 
IPL Project Report

1. Introduction
The Indian Premier League (IPL) is one of the most popular and competitive T20 cricket leagues globally. Cricket fans worldwide eagerly anticipate the Indian Premier League each year, which has grown into one of the most popular and prestigious T20 cricket leagues globally. The IPL brings together top-notch cricketers from various countries, making it a highly competitive tournament. 
In this project, we will analyze the batting and bowling performances of players across different IPL seasons. we conduct a comprehensive analysis of player performance based on batting and bowling data, aiming to gain valuable insights and recommend the best players for each position in a cricket team. The analysis includes visualizations, statistics, and player recommendations for forming a cricket team.
2. Data Loading
We started by loading the batting and bowling datasets for different IPL seasons. The data was read from CSV files and converted into structured data for further analysis.
To ensure accurate and reliable results, we started by collecting historical IPL data from reputable sources such as Kaggle and cricket databases. The datasets encompassed detailed statistics of players batting and bowling performances, including metrics like runs scored, strike rate, batting average, wickets taken, economy rate, and more. 
3. Data Cleaning
The initial step in the analysis involved data preprocessing to clean, format, and transform the raw data. Various preprocessing steps were performed, including handling missing values, duplicates, and inconsistencies. The data was standardized and normalized as required to ensure fair comparisons between players
The data was preprocessed to remove any missing or irrelevant entries, and the necessary Python libraries were used to read and manipulate the data effectively.
•	Replacing Dash with 0 in Batting "Avg" column: In the batting data, we replaced the dash  ("-") with 0 to handle missing values in the batting average column.
•	Replacing Star with Space in Batting "HS" column: In the batting data, we replaced the star    ("*") with (“  ”) to handle missing values in the Highest Score(HS) column.
•	Removing Unnecessary Columns: We removed irrelevant columns like "pos," "BBI," and "POS" from the batting and bowling datasets.
•	Combining Data Across Seasons: We combined batting and bowling data across different seasons for each player to obtain cumulative statistics.
•	Formatting Bowling Data: We calculated and formatted the average, economy rate, and strike rate for bowlers across different seasons.
4. Exploratory Data Analysis (EDA)
Exploratory Data Analysis (EDA) is a critical phase of any data analysis project, as it helps us comprehend the data and extract meaningful insights.
In this section, an exploratory data analysis was conducted to gain insights into the dataset. Summary statistics and data visualizations, such as graphs and charts, were used to understand the distribution of key variables. The analysis provided a comprehensive understanding of the players' performances in previous IPL seasons.
The dataset consists of detailed player information, such as their name, team, batting stats (runs, strike rate, average, 100s, 50s, 4s, 6s), and bowling stats (wickets, economy, average, 4-wicket hauls, 5-wicket hauls).
1.	Bar graphs: Used to visualize players with the strike rate, batting average, and the runs, centuries, half-centuries, fours, and sixes. These visualizations provided a clear understanding of the players performance in different categories.
2.	Pie charts: Depicting players with the most runs, centuries, half-centuries, four, sixes, wickets and 4-wicket/5-wicket hauls.
3.	Scatter plots: Utilized to explore the relationship between strike rate and batting average. This helped us identify trends and patterns that could indicate players consistency and effectiveness.
4.	Histograms: Employed to understand the distribution of player performances in terms of runs scored and wickets taken. The histograms helped identify outliers and players with exceptional performances.

5. Data Insights
A.	Batting Analysis:
Strike rate and batting average:
•	We analyzed the strike rate of players and found that several players have a strike rate above 145.0, indicating their aggressive style of play.
•	The top 30 players with the highest strike rates were identified and plotted to visualize their performance.
•	We also explored players with a batting average above 40.0, highlighting their consistency in scoring runs.
The top 30 players with the highest batting averages were plotted to identify the most consistent batsmen in IPL.
Runs and Centuries:
•	We analyzed the total runs scored by players in IPL and identified the players with more than 2000 runs.
•	The players with centuries were highlighted, showcasing their ability to score big and impactful innings.

Runs and Centuries:
•	We analyzed the total runs scored by players in IPL and identified the players with more than 2000 runs.
•	The players with centuries were highlighted, showcasing their ability to score big and impactful innings.
Half-Centuries, Fours, and Sixes:
•	Players with more than 15 half-centuries were identified, indicating their ability to consistently contribute with good scores.
•	We also explored players with more than 200 fours and those with more than 100 sixes, showcasing their boundary-hitting skills.


B.	Bowling Analysis:
Strike rate and Bowling average
•	Players with more than 20 wickets were analyzed, showcasing their effectiveness in taking wickets.
•	We also explored players with a strike rate above 40, highlighting their ability to strike at regular intervals.
•	Players with a bowling average above 60 were identified, emphasizing their skill in maintaining a low average.
Economy Rate and Wickets:
•	Players with an economy rate below 8 and innings more than 80 were identified, showcasing their ability to control the run flow.
•	The top 20 players with the most wickets were listed, highlighting the most successful bowlers in IPL.
4-Wicket and 5-Wicket Hauls:
•	Players with 4-wicket and 5-wicket hauls were identified, showcasing their ability to take a significant number of wickets in an innings.
C.	Batting Statistics
We analyzed the combined batting data to gather some summary statistics. Here are some key observations:

•	Total Number of Players: 338
•	Total Number of Seasons: 7
•	Total Matches Played: 1496
•	Total Innings Played: 1478
•	Total Runs Scored: 50920
•	Total Centuries: 97
•	Total Half-Centuries: 363
•	Total Fours: 5368
•	Total Sixes: 1896
•	Average Strike Rate: 126.96
•	Average Batting Average: 25.49
D.	Bowling Statistics
We analyzed the combined and formatted bowling data to gather some summary statistics. Here are some key observations:

•	Total Number of Players: 227
•	Total Number of Seasons: 7
•	Total Matches Played: 1346
•	Total Innings Bowled: 2263
•	Total Overs Bowled: 4735.4
•	Total Runs Conceded: 5575
•	Total Wickets Taken: 213
•	Total 4-Wicket Hauls: 14
•	Total 5-Wicket Hauls: 3
•	Average Economy Rate: 7.45
•	Average Bowling Average: 26.19
•	Average Strike Rate: 16.99
6. Player Selection criteria
Top Batsmen
Batsmen are the backbone of any team and should be consistent in scoring runs at a good strike rate.
Players who have scored more than 2500 runs, with a strike rate between 125 and 200, and a batting average above 40 are recommended for the batsmen position.
We identified top batsmen based on the following criteria:
1.	Runs scored: More than 2500
2.	Strike Rate: Between 125 and 200
3.	Batting Average: More than 40
Top Bowlers
Bowlers play a vital role in restricting the opposition and taking wickets.
Players with 70 or more wickets, an economy rate of less than 5.0, and an average below 4.0 are recommended for the bowler position. 
We identified top bowlers based on the following criteria:
1.	Wickets taken: More than 70
2.	Economy Rate: Less than 4.0
3.	 Bowling Average: Less than 5.0
Top All-Rounders
All-rounders play a crucial role in T20 cricket as they contribute with both bat and ball.
Players who have scored between 1500 and 2500 runs, with a strike rate above 145, and have hit between 78 and 200 sixes are recommended for the all-rounder position.
We identified top all-rounders based on the following criteria:
1.	Runs scored: Between 1500 and 2500
2.	Strike Rate: More than 145
3.	Sixes: Between 78 and 200
7. Cricket Team Selection
After identifying top performers in each category, we selected the best cricket team with the following composition:
•	All-Rounders -2
•	Batsmen - 5
•	Bowlers - 4
Now, it’s made the complete IPL cricket team.
8. Player Recommendations 
Forming a balanced cricket team requires players with diverse skills in both batting and bowling. To recommend the best players for each position, we defined specific criteria for selecting all-rounders, batsmen, and bowlers. Players who met these criteria were shortlisted for each category, ensuring a formidable lineup. Our final cricket team comprised the required number of players for each position, increasing the team’s chances of success.
9. Conclusion
The IPL project primary goal was to provide invaluable insights into player performances in T20 cricket. By conducting a thorough analysis of batting and bowling data, we identified players with exceptional skills and recommended the most suitable players for each position. This analysis is highly beneficial for IPL team owners, coaches, and cricket enthusiasts in forming a highly competitive cricket team capable of excelling in the IPL or any other T20 tournament.
