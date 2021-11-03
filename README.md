# Introduction

Currently, with Major League Baseball (MLB) sports sites, statistics and projections are only given in a tabular format. The data is, usually, only given using standard league settings. This tool is designed to accurately project MLB players' stats and rankings, and give the user the ability to put in their own league settings and get custom player projections and rankings based on those settings. Users have the freedom to select the factors they think are important to customize their own algorithm. This provides transparency to the user and gives them the ability to add or remove certain features that they believe should be part of the algorithm. In addition, one can visualize historic data and compare players using charts. Our platform offers the capability to study multiple players’ statistics with friendly, straightforward charts. With visual tools, we believe that it gives users efficient ways to digest data, make draft and in-season decisions, and find trends. 

---
# Installation
Steps for installing our fantasy baseball app:
1. In order to run our platform, Docker needs to be installed. The instructions to install Docker can be found in [Install Docker](https://docs.docker.com/get-docker/)

1. Once docker is installed, clone this domain to your local repository.

1. use the terminal/command prompt to go into the fantasy_app directory.

1. Once in the directory, run docker-compose up. For example, if the zip file was in the Downloads directory
```bash
cd Downloads/CODE/fantasy_app
```
5. The following commands would be used to build the application, 
```bash
docker-compose up -d
docker build .
```

6. The containers for the app and the MySQL database will start building. Once the two containers finish building, the application will automatically start.  


7. The application can be accessed at the following url on your browser:

``` javascript
localhost:8080
```


8. This url will lead to the application's home page. This application will present our projections, but the analysis and models used can be found at [analysis/models report](https://github.com/cse6242teamsport/fantasy_baseball)

![home](https://github.com/hoseela41/Fantasy_baseball_website/blob/main/img/home.png?raw=true)

---
# Fantasy APP functions
​
## Projected statistics for players in 2020 
​
After selecting the batters or pitchers at the home page, there will be a table with projected statistics and ranks for each player in 2020 based on the risk and categories selected. On this page, the following functions are offered:
​
- Risk tolerance selection: **selection bar** is used for picking low, medium or high risk in ranking players
​
- Choose stats to rank player: Check the categories in the **boxes** and hit **rank player** button to have the table shown based on the user-defined stats, the default sorting order is determined by projected rank. At least 4 categories are required to rank players.

-  Sorting table: The table could be resorted by any stats by clicking the **header** in the first row of table, for example, click **HR**, then the table will be sorted in ascending or descending order by the amount of HRs.
​
![sort_hr](https://github.com/hoseela41/Fantasy_baseball_website/blob/main/img/sort_hr.png?raw=true)

## Career statistics for individual player
​
There is also functionality to view historical data for an player. The application gives the ability to:

- View a player's career statistics: After clicking on a **player's name**, a table will display the stats of each season in his career. This table also supports the functionality of sorting by clicking on the **header** of each column.
![player_stat](https://github.com/hoseela41/Fantasy_baseball_website/blob/main/img/select_stat.png?raw=true)

- Visualization chart on specific category: To easily view trends of a player's performance, each category can be visualized to see the player's performance throughout their career. This is done by selecting a **category** that user would like to view, and clicking the **graph** button.
![visual_hr](https://github.com/hoseela41/Fantasy_baseball_website/blob/main/img/hr_stats.png?raw=true)​

## Player comparison
​
Our application offers the ability to compare two players' performance with a chart:
​
- Compare two players: First, check the boxes in the column of **Compare** for two players that user would like to compare, and hit the **Compare Players** button. 
![player_compare](https://github.com/hoseela41/Fantasy_baseball_website/blob/main/img/compare_players.png?raw=true)

- Second, choose the season in the **selection bar** and check the categories in the **boxes** that user intends to compare. 
![select_compare_stat](https://github.com/hoseela41/Fantasy_baseball_website/blob/main/img/select_compare.png?raw=true)

- Finally, click the **Compare These Stats** button. A bar chart with the categories chosen will appear. This offers the user the ability to visually compare player performance rather than comparing raw data.
​![compare_graph](https://github.com/hoseela41/Fantasy_baseball_website/blob/main/img/compare_graph.png?raw=true)
