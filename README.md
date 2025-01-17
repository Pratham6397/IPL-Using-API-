IPL API-Based Dashboard

Problem Statement
This API-based dashboard helps IPL teams and stakeholders understand player performances, team standings, and key metrics throughout the IPL 2024 season. It provides real-time insights into areas needing improvement and strategies to enhance team performance by using API to collect real-time data.

Steps Followed 

Step 1: Integrate API data into Power BI Desktop.

Get Data: Open Power BI Desktop and navigate to the "Home" tab. Select "Get Data" and choose "Web".

API Key Integration: Input the API endpoint URL along with your API key

"https://cricbuzz-cricket.p.rapidapi.com/"

Step 2: Open Power Query Editor and ensure thorough data profiling.

Enable "Column Distribution," "Column Quality," and "Column Profile" under the Data Preview section.

Select "Column Profiling Based on Entire Dataset."

Step 3: Handle any errors and empty values in specific columns like "Match Results" or "Player Statistics".

Step 4: Calculate average metrics (e.g., runs, wickets) considering valid data entries.

Step 5: Apply a visually appealing theme for the report.

Step 6: Add visuals representing player and team statistics.

Bar Charts: Visualize match results and player contributions.

Pie Charts: Represent player contributions.

Step 7: Use slicers for fields like "Teams," "Players," "Match Venue," and "Season".

Step 8: Create card visuals for key metrics like "Total Runs," "Total Wickets," and "Average Strike Rate."

Step 9: Incorporate visual filters to exclude null and zero values.

Step 10: Utilize line charts to depict trends in player and team performances.

Step 11: Add text boxes for titles, team names, and significant highlights.

Step 12: Insert shapes and images for branding elements like team logos and sponsor details.

Step 13: Use DAX expressions to create calculated columns for identifying the team currently batting and the runs needed to win.

           " Current_Batting_Team_Name = IF([Total_Inning]>1,[Inning_two_Team],[Inning_One_Team]) "

Step 14: Generate measures to calculate totals and percentages, such as "Total Matches Played" and "Win".


Step 15: Summarize key metrics like "Total Runs Scored" and "Total Wickets Taken" using card visuals.

Step 16: Publish the report to Power BI Service.

![Screenshot (3)](https://github.com/user-attachments/assets/72c7c442-fce0-4835-86c3-18a948e44b11)


IPL Dashboard Insights
A single-page report created on Power BI Desktop, published to Power BI Service, yields these insights:

[1] Total Runs and Wickets
Total Runs Scored

Total Wickets Taken

[2] Player Performance
Batsmen: Player1, Player2, Player3

Bowlers: PlayerA, PlayerB, PlayerC

[3] Team Standings
Teams Wins: Team

Teams Losses: Team

[4] Key Metrics
Average Runs per Match: 160.5

Average Wickets per Match: 8.2

[5] Additional Insights

Total Strike Rate:

Player1: 150.8

Player2: 145.2

Player3: 138.6

IPL Points:

Team1: 18 points

Team2: 16 points

These insights help identify strong performers, strategize team compositions, and enhance overall gameplay for better results in upcoming seasons.
