# Cricket League Database Management System

This project is a comprehensive Cricket League Database Management System implemented in Microsoft SQL Server. It includes the schema creation, data insertion, and various SQL queries to extract insightful information regarding players, teams, matches, and stadiums.

## Features

1. **Database Structure:**
   - The project defines and creates the following tables:
     - `Player`: Stores player information such as name, age, and role.
     - `Team`: Holds team details including team name, home stadium, and number of wins.
     - `Match`: Logs match details including match type, date, and teams.
     - `Stadium`: Records stadium information like capacity and name.
     - `Performance`: Tracks player performances for each match.
     - `Winner`: Logs match results and winning teams.

2. **Data Insertion:**
   - The project includes the insertion of sample data (at least 20 rows) into each table, allowing for simulation and testing of the queries.

3. **SQL Queries:**
   - A total of 23 SQL queries are provided, covering:
     - Player and team performance analysis.
     - Stadium-specific match statistics.
     - Aggregation of runs and wickets by players and teams.
     - Winning team identification.
     - Grouping and filtering of data for meaningful insights.

### Key SQL Queries
- **Top Players by Catches**: Find the player with the highest number of catches.
- **Team Home Stadiums**: List all teams and their respective home stadiums.
- **Average Runs per Team**: Calculate the average runs scored by players in each team.
- **Players with Over 50 Runs and 3 Wickets**: Find players who scored more than 50 runs and took at least 3 wickets in a match.
- **Teams with the Most Wins**: Identify teams with more than a certain number of wins.
- **Top Performers in Final Matches**: List top 3 players with the most runs scored in final or playoff matches.
- **Players Who Contributed to Team Wins**: Identify players whose individual performance was pivotal in securing wins for their team.

### Advanced Concepts Used:
- **Correlated Nested Queries**: Applied for performance comparison.
- **UNION**: Combines results from multiple queries.
- **GROUP BY with Aggregation**: Used for calculating statistics based on teams and players.
- **LIKE Operator**: Utilized for pattern matching in player names.
- **HAVING Clause**: Filters results based on aggregated data.

## Database Schema

The main entities in the system include:

- **Player** (`playerid`, `playername`, `age`, `playerrole`, `teamname`)
- **Team** (`teamid`, `teamname`, `homestadium`, `numberofwins`)
- **Match** (`matchid`, `matchtype`, `matchdate`, `teamid1`, `teamid2`, `stadiumid`)
- **Stadium** (`stadiumid`, `stadiumname`, `capacity`)
- **Performance** (`performanceid`, `playerid`, `matchid`, `runsscored`, `wicketstaken`, `catches`)
- **Winner** (`winnerid`, `matchid`, `winningteam`)

## Requirements

- Microsoft SQL Server or any compatible SQL environment.
- Basic understanding of SQL for executing the queries.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
