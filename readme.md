## Title

SteamRanking

### List of team members

Yujie Lu, Yizhuo Tan, Jinzhao Wu

### Problem Description

Steam has emerged as the largest and most diverse platform for PC gaming, boasting an extensive catalog of games spanning various genres, styles, and developers. While the variety of options is a testament to the platform's success, it has also presented a significant challenge: How do players navigate through this vast sea of games to find titles that match their interests and preferences? Many high-quality, niche, or indie games often go unnoticed due to a lack of visibility within the Steam ecosystem.
The problem is important because The gaming industry is a multi-billion-dollar market, and its success depends on both players' satisfaction and developers' ability to reach their intended audience. Currently Steam has over 90 thousand games on sale. Inefficient game discovery can impact the industry's economic stability.

### System Features

- Show ranking of ratings for each mainstream game category
- Show ranking of ratings filtered by the number of players
- Show ranking filtered by price or popularity
- Show ranking of developers and gamers
These features would be very helpful for gamers to find the games they need.

### Technology Stack

- Database: mysql

- Frontend & backend: flask with some frontend templates

- Data source: 
  - https://steamcommunity.com/dev
  - https://developer.valvesoftware.com/wiki/Steam_Web_API



#### Justification for Technology Choices 

Since we all use python and C/C++, flask is a decent choice for backend. And mysql is a popular DBMS that meets our needs.
We don’t know much about frontend, a good frontend template that could display the information should do the work.




#### Team Skills 

- Yujie Lu: C++/C, python, java
- Yizhuo Tan:C, python
- Jinzhao Wu: C++/C, python

#### System Specification

##### Entity:

- Gamer (player_id, gamesnum, name)
- Game (appid, rating, playernum, price, category, developer)
- Developer (developer_id, gamesnum, name)



##### Relationship

- Rating (id, appid, is_recommended, comment)
- developGame (developer_id, appid, )

- ownGame(player_id, appid)

